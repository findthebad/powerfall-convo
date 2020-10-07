# Find the Bad: Powerfall Convo
This lab continues to build on the previous [exercise](https://github.com/findthebad/model-3).  It should only require the installation of Docker and Docker Compose. 

## Disclaimer
This lab is based on real data containing actual malicious indicators.  If you attempt to do things such as find and run files, or visit network entities that occur in these logs, you do so at your own risk.

## Setup
1) Download and install [Docker](https://www.docker.com/get-started).
2) Download and install [Docker Compose](https://docs.docker.com/compose/install/) (On Windows Docker Compose should be bundled with the Docker installer, so this step shouldn't be required).
3) Download or clone this repository.
4) Open up a command prompt, make your way to this repository folder on your local machine and run `docker-compose up`.
5) When `docker-compose up` is finished bringing the containers up, open a browser and navigate to `http://localhost:5601` to access the Kibana instance.

## The Lab
This lab continues with the use of Kibana for identifying and investigating signs of a compromise (see [Model 3](https://github.com/findthebad/model-3)).  The `VT Hunting` dashboard has been updated with some new visualizations that should provide you the information you need to get started.

### Questions
1) What malicious domain has a process attempted to communicate with?
2) What were the command line arguments of the process that initiated the communication (Hint: There may be multiple processes, but only one that was "user" initiated)?
3) What do the arguments do? Can you decode all of them?
4) Does it appear the command was successful?  Why or why not?
5) When did this process activity start, end, and who was the user on what computer? 

Bonus:
What advanced persistent threat (APT) has been discussed as being the potential group behind this domain? 

### Useful Links
- [VirusTotal](https://www.virustotal.com/gui/home/upload)
- [Sysmon Event ID 22](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon#event-id-22-dnsevent-dns-query)
- [Base64](https://en.wikipedia.org/wiki/Base64)
- [CyberChef](https://github.com/gchq/cyberchef)
- [PowerShell](https://ss64.com/ps/powershell.html)
- [Investigating PowerShell Attacks](https://redcanary.com/blog/investigating-powershell-attacks/)

### Solution
Available [here](https://findthebad.com/powerfall-convo/).