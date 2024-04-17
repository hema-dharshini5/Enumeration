# Enumeration
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
## Output:
![Screenshot 2024-04-16 223519](https://github.com/hema-dharshini5/Enumeration/assets/147117728/8d563be0-7631-4ad9-82ae-20f1d9c5f9dd)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output:
![Screenshot 2024-04-16 223727](https://github.com/hema-dharshini5/Enumeration/assets/147117728/6af3ad70-ad6b-426c-922f-5f3d63046f74)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## Output:
![Screenshot 2024-04-16 224018](https://github.com/hema-dharshini5/Enumeration/assets/147117728/c8523cbe-f24e-4a20-9ba8-a4df379b7849)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## Output:
![Screenshot 2024-04-16 224122](https://github.com/hema-dharshini5/Enumeration/assets/147117728/bd605c04-981c-46c9-a650-c22237906212)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## Output:
![Screenshot 2024-04-16 224304](https://github.com/hema-dharshini5/Enumeration/assets/147117728/e593dbaa-15f0-4034-92e0-19811d44c8cf)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## Output:
![Screenshot 2024-04-16 224359](https://github.com/hema-dharshini5/Enumeration/assets/147117728/99e3b65d-cc18-430c-aa8e-926889c931f5)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![Screenshot 2024-04-17 082735](https://github.com/hema-dharshini5/Enumeration/assets/147117728/204c5833-85a2-4423-983d-419dc45eac99)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![321864522-6034435c-b383-491b-b814-f1a6b7e4548c](https://github.com/hema-dharshini5/Enumeration/assets/147117728/b13902a9-3f12-43ea-a88c-fcb92d41c160)







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
  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

