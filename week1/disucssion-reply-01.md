
# response to class discussion

Craigen,

Very good choice of articles. Thanks for giving a writeup. I am a database architect and administrator, and this kind of thing keeps me up at night. Brother McLaughlin wrote a nice encryption data type and posted it to his blog. It's for Oracle, but live encryption could be ported to just about any database. Some databases like MongoDB have something like this built-in, where other databases do not. My thought are to use Postgres 16 because it is the most extensible database in the world, and because it is gaining so much popularity.

```sql
# ubuntu 22 or 24
sudo apt-get install postgresql-plpython3-16
su - postgres
psql
create extension plpython3u;

create type encrypted_text as (
    ciphertext bytea
,   bitmask    int
);

create table users (
    id              bigserial primary key
,   name            jsonb
,   pii             encrypted_text
...
,   encryption_mask int
);
```

Then, you would need to create two procedures, one for encryption and the other for decryption. Finally, your programs would compare the the bitmask column in the data type and your user (encryption_mask). If the masks matched, then the user would see the data, else the data would remain encrypted. I am working on this concept in an application I am building, so I can't share much more than this. Using live encryption like this would certianly prevent hackers (un-knowing) from simply slurping pii information. It would not stop an internal hacker or one that had spent sufficient time in your network from getting the data, provided that they could get access to the decyper keys.
