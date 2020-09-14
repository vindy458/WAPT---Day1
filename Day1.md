# <a style="color:lightBlue">#Day1 Tutorial </a>

---
###### Topics: Linux Commands, DNS Records, Information Gathering

## Linux commands


<b> 1. Head Command: </b>

- The head command reads the first ten lines of a any given file name. 
  
  
- Command will display the first ten lines of the file named ‘/etc/passwd‘
``` bash 
     #head /etc/passwd  
```

- Head will show the first ten lines of each file separately. For example, the following command will show ten lines of each file
```bash 
    # head /etc/passwd /etc/shadow
```
For Reference:
``` 
https://www.tecmint.com/view-contents-of-file-in-linux/
```
<b> 2. Tail Command:</b> 
- command will print the last ten lines of a file called ‘access.log‘.
  
```bash 
    # tail access.log  
```

- If more than one file is provided, tail will print the last ten lines of each file as shown below.
```bash 
    # tail access.log error.log
```

<b> 3. cat Command: </b>

Each line in /etc/passwd file represents an individual user account and contains following seven fields separated by colons :).

<img src= "https://www.computernetworkingnotes.org/images/linux/rhce-study-guide/rsg02-02-etc-passwd-file.png">

 
   * Username or login name 
   * Encrypted password
   * User ID
   * Group ID
   * User description
   * User’s home directory
   * User’s login shell

<img src= https://landoflinux.com/images/etc_passwd.png>


<b>For Reference:</b>
```
https://landoflinux.com/linux_adding_users_groups.html
```

- The /etc/passwd file is stored in /etc directory. To view it, we can use any regular file viewer command such as cat, less, more, etc.
```bash
    # cat /etc/passwd 
```
---
## DNS Records

<strong>DNS Types: 10 Top DNS Record Types </strong>

###### DNS servers create a DNS record to provide important information about a domain or hostname, particularly its current IP address. The most common DNS record types are:

* <b>Address Mapping record (A Record) </b>
    *   also known as a DNS host record, stores a hostname and its corresponding IPv4 address.
  
*  <b>IP Version 6 Address record (AAAA Record)</b>
   *  stores a hostname and its corresponding IPv6 address.
    
* <b>Canonical Name record (CNAME Record)</b>
  * can be used to alias a hostname to another hostname. When a DNS client requests a record that contains a CNAME, which points to another hostname, the DNS resolution process is repeated with the new hostname.
* <b>Mail exchanger record (MX Record)</b>
     *  specifies an SMTP email server for the domain, used to route outgoing emails to an email server.
* <b>Name Server records (NS Record)</b>
  * specifies that a DNS Zone, such as “example.com” is delegated to a specific Authoritative Name Server, and provides the address of the name server.
* <b>Reverse-lookup Pointer records (PTR Record)</b>
  * allows a DNS resolver to provide an IP address and receive a hostname (reverse DNS lookup).
* <b>Certificate record (CERT Record)</b>
  * stores encryption certificates—PKIX, SPKI, PGP, and so on.
* <b>Service Location (SRV Record)</b>
  * a service location record, like MX but for other communication protocols.
*  <b>Text Record (TXT Record)</b>
   *  typically carries machine-readable data such as opportunistic encryption, sender policy framework, DKIM, DMARC, etc.
* <b>Start of Authority (SOA Record) </b>
  * this record appears at the beginning of a DNS zone file, and indicates the Authoritative Name Server for the current DNS zone, contact details for the domain administrator, domain serial number, and information on how frequently DNS information for this zone should be refreshed.

---
## Information Gathering

#### Websites

* shodon.io
* censys.io
* crt.io
* archieve.org 
* mxtoolbox.com
* kitterman.io
* greynoise.io
* hunter.io
* recon.dev
* spiderfoot.net <b>(OSINT)</b>

#### Tools:
  * dig
  * nmap
  * amass
  * aquatone
  * sublist3r
  * gobuster (dir bruteforce)


