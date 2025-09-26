<img width="780" height="787" alt="image" src="https://github.com/user-attachments/assets/00717dbf-055d-402b-be63-e6d321937865" /># Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
**output**
<img width="1178" height="963" alt="image" src="https://github.com/user-attachments/assets/beb71cc3-d67b-49f4-a289-e23e2c4aee71" />


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
**output**
<img width="911" height="967" alt="image" src="https://github.com/user-attachments/assets/08151885-aeae-4937-8dc8-c9b13f6fe17f" />


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
**output**
<img width="1035" height="771" alt="image" src="https://github.com/user-attachments/assets/f09d1575-01b0-4d4b-b940-4d34579fddd2" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
**output**
<img width="1309" height="831" alt="image" src="https://github.com/user-attachments/assets/af069c8a-f501-4680-ab57-b5b69ee21cfb" />


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
**output**
<img width="964" height="974" alt="image" src="https://github.com/user-attachments/assets/9101fbdc-d438-40a6-8248-363e7881a542" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
**output**
<img width="958" height="958" alt="image" src="https://github.com/user-attachments/assets/f6850419-0dcc-4290-a5da-2e275db20106" />


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
**output**
 <img width="1777" height="937" alt="image" src="https://github.com/user-attachments/assets/5755ae26-f6bb-4bea-ac13-e12c3f362a37" />

#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="589" height="128" alt="image" src="https://github.com/user-attachments/assets/8caddac5-cfb3-41fe-96d6-5fb84f544c6f" />

<img width="589" height="128" alt="image" src="https://github.com/user-attachments/assets/f71ab738-fc9c-425b-b2a4-17e6b5820683" />

<img width="662" height="457" alt="image" src="https://github.com/user-attachments/assets/6d57e0d5-1c08-4f5d-8272-23e7e39d0451" />





##dnsenum
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


##smtp-user-enum

Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  <img width="647" height="355" alt="image" src="https://github.com/user-attachments/assets/d1eb5487-0303-470d-b93a-00fad3b240f1" />

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="527" height="177" alt="image" src="https://github.com/user-attachments/assets/0f42aedf-df3a-4a3f-87a6-8dc19c163856" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

