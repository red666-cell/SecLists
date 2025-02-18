# Web discovery wordlists

## AdobeCQ-AEM.txt
Use for: Discovering sensitive filepaths of **Adobe Experience Manager**
Creation date: Oct 1, 2017
No updates have been made to this wordlist since its creation.

## AdobeXML.fuzz.txt
Use for: Discovering sensitive filepaths of **Adobe ColdFusion**
Creation date: Aug 27, 2012
No updates have been made to this wordlist since its creation.

## CGI-HTTP-POST-Windows.fuzz.txt
Use for: Exploiting various vulnerabilities in the now defunct WYSIWYG HTML editor and website administration tool, [Microsoft FrontPage](https://en.wikipedia.org/wiki/Microsoft_FrontPage)
Source: https://github.com/deepak0401/Front-Page-Exploit
Date of last update: Aug 27, 2012
The last version of FrontPage was released on 2003.

## CGI-HTTP-POST.fuzz.txt
Use for: Exploiting/Discovering various vulnerabilities in extremely old systems (Circa 1998) that use "CGI". 
Date of last update: Aug 27, 2012

This wordlist tests for the following vulnerabilities:
- Default password in the [Nortel Meridian](https://en.wikipedia.org/wiki/Nortel_Meridian) private branch exchange **telephone switching system**. Source: [Nikto](https://github.com/sullo/nikto/blob/07653b73cb711972df72a8c66191468705a9b14e/program/databases/db_tests#L1167).
- XSS in the **"Bajie HTTP JServer"** (software site completely defunct, no archives exist). Source: [Nikto](https://github.com/sullo/nikto/blob/07653b73cb711972df72a8c66191468705a9b14e/program/databases/db_tests#L803)
- CGI Vulnerability in an unknown system (payload `lastlines.cgi?process`) which would allow attackers to "read arbitrary files and/or execute commands". Source: [Nikto](https://github.com/sullo/nikto/blob/07653b73cb711972df72a8c66191468705a9b14e/program/databases/db_tests#L1036)
- Remote File Include in **[myPHPNuke](https://web.archive.org/web/20140812223623/http://www.myphpnuke.com/)**. Source: [Nessus](https://www.tenable.com/plugins/nessus/11836)
- DoS in the **"D-Link Ethernet/Fast Ethernet Print Server DP-300+"**. Source: [Sullo's Security Advisory Archive](https://raw.githubusercontent.com/sullo/advisory-archives/master/phenoelit.de_dp-300.txt).

## CGI-Microsoft.fuzz.txt
Use for: Exploiting/Discovering various vulnerabilities in miscelaneous CGI scripts that run on Microsoft operating systems.
Date of last update: Aug 27, 2012

## raft-* wordlists
Use for: Directory and file brute-forcing leading to identification of vulnerabilities in web applications.
Source: [Google's RAFT](https://code.google.com/archive/p/raft/)

## combined_words.txt

Use for: discovering files    
This list is automatically updated by a github action whenever any of the lists it's composed by is modified.

This list is a combination of the following wordlists:

- big.txt
- common.txt
- raft-large-words-lowercase.txt
- raft-large-words.txt
- raft-medium-words-lowercase.txt
- raft-medium-words.txt
- raft-small-words-lowercase.txt
- raft-small-words.txt


## combined_directories.txt

Use for: discovering files and directories    
This list is automatically updated by a github action whenever any of the lists it's composed by is modified.

This list is a combination of the following wordlists:
- apache.txt
- combined_words.txt
- directory-list-1.0.txt
- directory-list-2.3-big.txt
- directory-list-2.3-medium.txt
- directory-list-2.3-small.txt
- raft-large-directories-lowercase.txt
- raft-large-directories.txt
- raft-medium-directories-lowercase.txt
- raft-medium-directories.txt
- raft-small-directories-lowercase.txt
- raft-small-directories.txt
- common_directories.txt

### Usage
Use for: discovering files and directories

### Source
This list is automatically updated by a GitHub action whenever any of the lists it's composed by is modified.


## dsstorewordlist.txt

SOURCE: https://github.com/aels/subdirectories-discover

Perfect wordlist to discover directories and files on target site with tools like ffuf.
- It was collected by parsing Alexa top-million sites for **.DS_Store** files (https://en.wikipedia.org/wiki/.DS_Store), extracting all the found files, and then extracting found file and directory names from around 300k real websites.
- Then sorted by probability and removed strings with one occurrence.
- resulted file you can download is below. Happy Hunting!

## vulnerability-scan_j2ee-websites_WEB-INF.txt
Use for: discovering sensitive j2ee files exploiting a lfi

References: 
    
- https://gist.github.com/harisec/519dc6b45c6b594908c37d9ac19edbc3
- https://github.com/projectdiscovery/nuclei-templates/blob/master/vulnerabilities/generic/generic-j2ee-lfi.yaml
- https://github.com/ilmila/J2EEScan/blob/master/src/main/java/burp/j2ee/issues/impl/LFIModule.java


## Microsoft-Frontpage.txt
Use for: Fuzzing for common filepaths in webpages designed with **[Microsoft Frontpage](https://en.wikipedia.org/wiki/Microsoft_FrontPage)**

Year of the first release of Microsoft Frontpage: 1997

## Oracle-EBS-wordlist.txt
Use for: Fuzzing for common filepaths of [Oracle E-Business Suite](https://www.oracle.com/applications/ebusiness/) (EBS) version 11.

EBS v11 exposes:
- usernames
- ports
- OS information
- protocol information
- Unauthenticated file upload
- Cookie contents
- SHA-1 hashed passwords

As an Unauthenticated user it's also possible to:
- Create forms
- Get servlets status
- Get certain configuration files

Reference: https://the-infosec.com/2017/03/29/do-you-know-what-your-erp-is-telling-us/

Date of last update: Oct 7, 2019


<<<<<<< HEAD
## iis-systemweb.txt
Use for: Fuzzing the `/aspnet_client/system_web/` directory on [Microsoft IIS](https://www.iis.net/) servers to detect **CGIs** and **scripts** even even if the two ladder directories are inaccessible.

Reference: https://github.com/irsdl/IIS-ShortName-Scanner
Discussion: https://github.com/danielmiessler/SecLists/pull/783

Date of last update: Jun 27, 2022
=======
Date of last update: Oct 14, 2010
>>>>>>> 0a6cbb9c (feat(docs): Moved Web-Server wordlists into their own directory)
