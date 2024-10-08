# References for Questions Asked:
Ciampa, Mark. CompTIA Security+ Guide to Network Security Fundamentals. Available from: Brigham Young University - Idaho, (7th Edition). Cengage Learning US, 2020.
---
# Project 2-2 Activities and Questions:
## Step 5:
Read through the material. In your own words, how does the Mitre CVE compare with the NIST NVD? When would you use the CVE? When would you use the NVD? How frequently is the NVD updated? Is this often enough?

The two methods differ in detail and refresh speed. They update MITRE CVE entries continuously; however, they review each vulnerability to see if it qualifies for a CVE ID. I'm sure that takes some time. Saying that MITRE CVEs are instant is a mistake. It would be better to define how long MITRE takes to validate than to say the MITRE entries continuously.

On the other hand, NVDs, produced by NIST engineers, have a crucial update cadence of two hours. This frequent update ensures you always work with the most current information. NIST engineers typically add more detail in their NVD entries than MITRE engineers in their CVEs. NIST engineers add links to vendor websites, analyze the vulnerability, and give those vulnerabilities a severity score. NVDs are typically much better at helping you determine what vulnerabilities you need to work on first.

## Step 14
Click Description Summary Word to display a bar graph of the most common words used in a vulnerability description, as seen in Figure 2-10. Hover over the three highest bars to view the three most frequent words. Is this what you would have expected?

While a word frequency histogram may not seem significant initially, it can provide valuable insights. For instance, it shows how often NIST documentation uses the word 'vulnerability' instead of 'exploit' (159,405:20,718, respectively). This chart exposes one point of interest: their scrutiny on qualifying vulnerabilities as exploits. It's a small detail but can lead to a deeper understanding of the data.

## Step 16
Return to the NVD Visualizations page. Click Products – CPE. Which vendor has the highest total products appearing in the NVD? View other vendors by hovering over the bars. What do you find interesting about this distribution?

Ah! Hah! There is a graph I can delve into. CISCO has 33,659 known vulnerabilities. This graph doesn't show that CISCO is lazy or careless in its software releases. On the other hand, I know they are a trusted vendor; however, hackers attack them much more than Schneider-Electric, which hovers around 
2620 vulnerabilities. Cisco is also a large company with many products. Attack surface size and usage are likely why Cisco has so many vulnerabilities.

[Back to Index](_overview.md)
