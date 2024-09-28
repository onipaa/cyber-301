# The CloudStrike Outage and Market-Driven Brittleness
- author: Barath Raghavan and Bruce Schneier
- document group: Lawfare
- date: July 25, 2024
- web: [CrowdStrike](https://www.schneier.com/essays/archives/2024/07/the-crowdstrike-outage-and-market-driven-brittleness.html)


Key Points:
- The catastrophe is yet another reminder of how brittle global internet 
  infrastucture is.
- The brittleness is not confined to technology.
- Redundant systems are often overlooked because of their cost vs return on 
  investment.
- Living on the edge (brittleness) is onl profitable when everything is working.
    - expenses of outages like this one far outweigh monies gained through 
      brittleness
- Cloudstrike was a buggy software update.
- The software was rolled out quickly because it was expensive to roll out
  traditionally
    - 1% (beta group)
    - 10% (first main release)
    - 100% (everyone)
  what they did
    - 100% (beta)
- If we build it right, our systems will be more resilient, and our code roll-
  outs will not cause catastrophic outages.

Missing Points:
- What really caused the outage. All OSes have:
    - ring 0 kernel level programs and drivers
        - Boot and OS control programs
        - Programs that run here have highest level of privileges.
        - Panics at this level == blue screen (windows), gray screen (linux), 
          and pink screen (osx)
        - The lock/panic protects applications and the system from doing bad 
          stuff to your data and the system itself.
        - Certification at this level takes a long time.
        - CloudStrike (main program) lives here.
    - ring 1 application level programs
        - CloudStrike addendums (this way CS gets away with not having to re-
          certify)
        - Addendums include configurations and bite-sized executable blocks of
          code.
        - The patch that took the world down was to these addendum files.
        - A file that was supposed to have information in it had no information.
          The overloard program (in the kernel) did not pre-check the files and
          panicked.
        - The overlord program forced a re-evaluation of the code every time the
          system booted, thereby killing the OS unless one could subvert the
          regular boot cycle.
        - Computers that had bitlocker and cloudstrike were borked without 
          clearing the CMOS, booting to a USB or other removable media, and then
          re-installing a fresh copy of the OS.



Question for Class:
- How many of you were affected directly by the CloudStrike release?
- What was your understanding of its cause?