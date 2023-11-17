# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

## AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

### Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

#### Google Hacking:
Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

#### site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
### OUTPUT: 

<img height=30% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/ea249868-8d4d-4346-8232-4004ce671f4a">

#### filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/13bac3df-7d58-40ea-803c-ff5fe8163c33">

#### intext:
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
### OUTPUT: 

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/8919a9cd-380d-47d2-9fea-6f9fb431feb3">

#### inurl:
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
### OUTPUT: 

 <img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/04f40d8b-d06e-4305-a8d0-003eeb2b7a17">
 
#### intitle:
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
### OUTPUT: 

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/cb3bbcd1-b4d5-40c1-8986-1c9ecf38ce7f">

#### link:
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
### OUTPUT: 

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/da4fc7f3-0104-456f-8f40-00fb26b67263">

#### cache:
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website. 
### OUTPUT: 
<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/af7e2a48-990c-4ecb-a46c-90fbf4ab70fc">

# DNS Enumeration
## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
### OUTPUT:

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/5da3f1d4-cfb2-4f67-af0b-a9253a43e379">

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/1e4a5945-10fa-42f7-b17f-30b8588a5e89">

## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
### OUTPUT: 

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/da9112df-2f42-4a94-8de6-0ba425e87f3a">

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
### OUTPUT: 

<img height=40% width=70% src="https://github.com/Vasanthamukilan/Enumeration/assets/119559694/ec656dc3-7682-4c59-8741-3a95a8f9079b">

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same
![12](https://github.com/Vasanthamukilan/Enumeration/assets/119559694/50a3b3bc-8aed-47da-a815-fd7b61154e5e)
# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands 
### Output
![13](https://github.com/Vasanthamukilan/Enumeration/assets/119559694/71890a29-5605-4bc0-9356-8d0fa5a3ea53)
## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
### OUTPUT:
![14](https://github.com/Vasanthamukilan/Enumeration/assets/119559694/0407f286-1346-43bc-bdde-b3fc4b20b91c)
## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

