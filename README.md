# CISCO CVE-2020-3452 Scanner & Exploiter

It will scan the target servers from shodan and then find the vulnerable servers to CVE-2020-3452 (Cisco Adaptive Security Appliance and FTD Unauthorized Remote File Reading).

## About 

A vulnerability in the web services interface of Cisco Adaptive Security Appliance (ASA) Software and Cisco Firepower Threat Defense (FTD) Software could allow an unauthenticated, remote attacker to conduct directory traversal attacks and read sensitive files on a targeted system.

The vulnerability is due to a lack of proper input validation of URLs in HTTP requests processed by an affected device. An attacker could exploit this vulnerability by sending a crafted HTTP request containing directory traversal character sequences to an affected device. A successful exploit could allow the attacker to view arbitrary files within the web services file system on the targeted device.

The web services file system is enabled when the affected device is configured with either WebVPN or AnyConnect features. This vulnerability cannot be used to obtain access to ASA or FTD system files or underlying operating system (OS) files.

## Prerequisites

Install [Shodan-Command-Line-Interface](https://cli.shodan.io/)

```
1. pip install -U setuptools
2. easy_install shodan
3. easy_install -U shodan
4. shodan init YOUR_API_KEY
```

## Usage

Linux

```
1. git clone https://github.com/darklotuskdb/CISCO-CVE-2020-3452-Scanner-Exploiter.git
2. cd CISCO-CVE-2020-3452-Scanner-Exploiter/
3. chmod +x SnE-CVE-2020-3452.sh
4. ./SnE-CVE-2020-3452.sh
```

### Screenshot
![SnE-CVE-2020-3452](https://user-images.githubusercontent.com/29382875/103662913-816c9e00-4f96-11eb-9d35-53a9767589e2.png)

## Reference

* https://twitter.com/aboul3la/status/1286012324722155525
* https://tools.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-ro-path-KJuQhB86

## Donation
[BuyMeACoffee](https://www.buymeacoffee.com/darklotus) if you like my work

## About Me

* **DarkLotus** - *Cyber Security Researcher* - [DarkLotusKDB](https://github.com/darklotuskdb)

### Social Media Handles
* [Twitter](https://twitter.com/darklotuskdb)
* [Medium](https://medium.com/@darklotus)
* [Linkedin](https://www.linkedin.com/in/kamaldeepbhati/)
* [Instagram](https://www.instagram.com/kamaldeepbhati/)
