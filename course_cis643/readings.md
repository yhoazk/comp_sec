# Schedule and Readings
[src](https://web.ecs.syr.edu/~wedu/Teaching/cis643/schedule.html)
## Introduction and Overview

    Overview of Computer Security (Lecture Notes: pdf) 

Vulnerabilities in General Software

    Unix Security Basics (Lecture Notes: pdf)
        Users and Groups.
        File Permissions: access control, umask, chmod, chown, chgrp, Set-UID. 
    Set-UID Programs and Vulnerabilities (Lecture Notes: pdf)
        Required Reading: Bishop: How to Write a Setuid Program
        Reading: Checklist for Security of Setuid Programs (a local copy) 
    Vulnerabilities and Attacks
    Lecture Notes: Buffer_Overflow.pdf   Race_Condition.pdf  
                   Input_Validation.pdf  Format_String.pdf  
        Buffer Overflow:
            Required Reading: Smashing The Stack For Fun And Profit (Aleph One)
            Heap Overflow: A heap of risk: Buffer overflows on the heap and how they are exploited 
        Format String
            Required Reading: Exploiting Format Strng Vulnerabilities (scut / team teso) 
        Race Condition:
            Required Reading: Secure programmer: Prevent race conditions (by David Wheeler) 
        Input Validation
            Required Reading: Chapter 5: Secure Programming for Linux and Unix HOWTO (by David Wheeler) 
        David Wheeler's book: Secure Programming for Linux and Unix HOWTO -- Creating Secure Software 

Web Security: Vulnerabilities and Access Control (Lecture Notes: pdf)

    Basics of Web Security
        HTML, HTML5, HTTP, HTTPS, JavaScript, Apache, PHP.
        Session ID, Cookies, DOM objects
        Same Origin Policy (SOP) 
    Vulnerabilities and Attacks
        Cross-Site Scripting (XSS) Attacks
            Required Reading: Cross-site Scripting from Wikipedia
            Required Reading: Cross-Site Scripting Worm and Virus
            News: Cross-Site Scripting Worm Floods MySpace
            Technical Details of the Samy Worm 
        Cross-Site Request Forgery (CSRF) Attacks
            Required Reading: Cross-Site Request Forgeries: Exploitation and Prevention (A local copy) 
        SQL Injection Attacks
            Required Reading: W3Schools: SQL Injection
            Steve Friedl's Unixwiz.net Tech Tips: SQL Injection Attacks by Example
            SQL Injection Comic
            OWASP's Top-10 List: The 10 Most Critical Web Application Security Vulnerabilities. 
        ClickJacking Attacks
            UI Redressing: Attacks and Countermeasures Revisited 
        Web Tracking and Privacy
            Required Reading: How Advertisers Use Internet Cookies to Track You (The Wall Street Journal, July 30, 2010).
            The Web's New Gold Mine: Your Secrets (The Wall Street Journal, July 30, 2010).
            Firesheep Highlights Web Privacy Problem (The Wall Street Journal, August 25, 2010).
            Facebook in Privacy Breach: Top-Ranked Applications Transmit Personal IDs, a Journal Investigation Finds (The Wall Street Journal, October 18, 2010).
            A Web Pioneer Profiles Users by Name (The Wall Street Journal, October 25, 2010). 
    Advanced Topic: Access Control in the Web. (Lecture Notes: ppt)
        Required Reading: Why Are There So Many Vulnerabilities in Web Applications?
        Escudo: A Fine-grained Protection Model for Web Browsers.
        Scuta: A Server-Side Access Control System for Web Applications. 
    Advanced Topic: Running Native Code inside Browsers.
        Google Chrome's Native Client
        Native Client: A Sandbox for Portable, Untrusted x86 Native Code, by Yee et al. 

System Security

    Access Control: Basic concepts (Lecture Notes: pdf)
        Access Control Matrix
        Access Control List (ACL) 
    Capabilities (Lecture Notes: pdf)
        Required Reading: Henry M. Levy, Capability-Based Computer Systems. (read chapter 1).
        (Case Study) White Paper: Trusted Solaris 8 Operating Environment. 
    Intel x86 Protection Mode (Lecture Notes: pdf )
        Intel 80386 Reference Programmer's Manual (Chapter 5.1, 6.3, and 8.3).
        Intel Architecture Software Developer's Guide (Chapter 4). 

