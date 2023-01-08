#  Software Vulnerabilities

An ongoing & curated collection of awesome software best practices and techniques, libraries and frameworks, E-books and videos, websites, blog posts, links to github Repositories, technical guidelines and important resources about  Software Vulnerabilities in Cybersecurity.
> Thanks to all contributors, you're awesome and wouldn't be possible without you! Our goal is to build a categorized community-driven collection of very well-known resources.

![cybersecurity](https://github.com/paulveillard/cybersecurity-vulnerabilities/blob/main/Img/vulnerabilitiies.png)

## Table of Contents
- [Introduction](#)
  - [What is a Vulnerability](#)
    - What is a Software Vulnerability?
    - How does a Software Vulnerability work?
    - What can an Attacker do with a Software Vulnerability?
    - What can cause a Software Vulnerability?
    - How can we deal with a Software Vulnerability?
  - [Examples of Software Vulnerabilities](#)
  - [List of Software Vulnerabilities](#)
  - [How to Prevent Software Vulnerabilities](#)
  - [Impact of Software Security Vulnerabilities](#)


## Introduction

### What is a Vulnerability?
- A vulnerability is a hole or a weakness in the application, which can be a design flaw or an implementation bug, that allows an attacker to cause harm to the stakeholders of an application. 
> Stakeholders include the application owner, application users, and other entities that rely on the application.

![threats](https://github.com/paulveillard/cybersecurity-threats/blob/main/Img/Vulnerability-Assessment-Idenitfying-Vulnerabilities.jpg)

### What is a Software Vulnerability?

A software vulnerability is a defect in software that could allow an attacker to gain control of a system. 
> These defects can be because of the way the software is designed, or because of a flaw in the way that it’s coded.



### How does a Software Vulnerability work?

An attacker first finds out if a system has a software vulnerability by scanning it. he scan can tell the attacker what types of software are on the system, are they up to date, and whether any of the software packages are vulnerable.
> When the attacker finds that out, he or she will have a better idea of what types of attacks to launch against the system. 
>> A successful attack would result in the attacker being able to run malicious commands on the target system.

### What can an Attacker do with a Software Vulnerability?

An attacker can exploit a software vulnerability to steal or manipulate sensitive data, join a system to a botnet, install a backdoor, or plant other types of malware.  Also, after penetrating into one network host, the attacker could use that host to break into other hosts on the same network.

![Software-vulnerability](https://github.com/paulveillard/cybersecurity-vulnerabilities/blob/main/Img/Zero-Day-Timeline.png)

### What can cause a Software Vulnerability?

### How can we deal with a Software Vulnerability?

### Examples of Software Vulnerabilities

- Lack of input validation on user input
- Lack of sufficient logging mechanism
- Fail-open error handling
- Not closing the database connection properly

### List of Software Vulnerabilities

##### Allowing Domains or Accounts to Expire

##### `Buffer Overflow`
- These allow someone to put more data into an input field than what the field is supposed to allow.  An attacker can take advantage of this by placing malicious commands into the overflow portion of the data field, which would then execute.

> Buffer overflow occurs when an attempt is made to store data that is too big for the memory space allocated. Attackers can use this software coding mistake, where the storage capacity of a program is overwritten, to take control of or to access your system. This vulnerability tends to be more common in software written in C and C++. Many programming languages have automatic protection against buffer overflow attacks.

#### `SQL Injection`
-  This could allow an attacker to inject malicious commands into the database of a web application.  The attacker can do this by entering specially-crafted Structured Query Language commands into either a data field of a web application form, or into the URL of the web application.  If the attack is successful, the unauthorized and unauthenticated attacker would be able to retrieve or manipulate data from the database.

#### `Third-Party libraries`
- Many programmers use third-party code libraries, rather than try to write all software from scratch.  This can be a real time-saver, but it can also be dangerous if the library has any vulnerabilities.  Before using any of these libraries, developers need to verify that they don’t have vulnerabilities.

#### `Application Programming Interfaces`
- An API, which allows software programs to communicate with each other, could also introduce a software vulnerability.  Many APIs are not set up with strict security policies, which could allow an unauthenticated attacker to gain entry into a system.

##### Business logic vulnerability
##### CRLF Injection
##### CSV Injection by Timo Goosen, Albinowax
##### Catch NullPointerException
##### Covert storage channel
##### Deserialization of untrusted data
##### Directory Restriction Error
##### Doubly freeing memory
##### Empty String Password
##### Expression Language Injection
##### Full Trust CLR Verification issue Exploiting Passing Reference Types by Reference
##### Heartbleed Bug
##### Improper Data Validation
##### Improper pointer subtraction
##### Information exposure through query strings in url by Robert Gilbert (amroot)
##### Injection problem
##### Insecure Compiler Optimization
##### Insecure Randomness
##### Insecure Temporary File
##### Insecure Third Party Domain Access
##### Insecure Transport
##### Insufficient Entropy
##### Insufficient Session-ID Length
##### Least Privilege Violation
##### Memory leak
##### Missing Error Handling
##### Missing XML Validation
##### Multiple admin levels
##### Null Dereference
##### OWASP .NET Vulnerability Research
##### Overly Permissive Regular Expression
##### PHP File Inclusion
##### PHP Object Injection by Egidio Romano
##### PRNG Seed Error
##### Password Management Hardcoded Password
##### Password Plaintext Storage
##### Poor Logging Practice
##### Portability Flaw
##### Privacy Violation
##### Process Control
##### Return Inside Finally Block
##### Session Variable Overloading
##### String Termination Error
##### Unchecked Error Condition
##### Unchecked Return Value Missing Check against Null
##### Undefined Behavior
##### Unreleased Resource
##### Unrestricted File Upload
##### Unsafe JNI
##### Unsafe Mobile Code
##### Unsafe function call from a signal handler
##### Unsafe use of Reflection
##### Use of Obsolete Methods
##### Use of hard-coded password
##### Using a broken or risky cryptographic algorithm
##### Using freed memory
##### Vulnerability template
##### XML External Entity (XXE) Processing

### How to Identify Software Vulnerabilities
The common methods of identifying vulnerabilities in a software project are:

- Source Code Scanning using automated tools that run against a source code repository or module, finding string patterns deemed to potentially cause security vulnerabilities.
 - Automated Penetration Testing (black/grey box) through penetrating testing tools automatic scans, where the tool is installed on the network with the web site being tested, and runs a set of pre-defined tests against the web site URLs.
- Manual Penetration Testing, again using tools, but with the expertise of a penetration tester performing more complicated tests.
- Secure Code Review with a security subject matter expert.

![vulnerabilities](https://github.com/paulveillard/cybersecurity-vulnerabilities/blob/main/Img/Survey_Vulnerabilities.png)

### How to Prevent Software Vulnerabilities
> These are some common ways to prevent software vulnerabiltiies (not a mitigation guideline)

#### 1. Test Your Software
It’s a good practice to test your software often as this will help you find and get rid of vulnerabilities quickly. You can test your software using code analysis tools, white box testing, black box testing, and other techniques.

#### 2. Update the Software Regularly
It is important to regularly update software as outdated software is prone to vulnerabilities. By making sure your software uses up to date components and dependencies, you can prevent security issues and software vulnerabilities.

#### 3. Set Up Software Design Requirements
Define a set of principles that need to be followed while developing each software release. These principles will show the developers how to write, inspect, and demonstrate their code to ensure security best practices are followed. Following the latest information from organizations such as CWE, OWASP, and CERT will also help you detect and prevent vulnerabilities.

#### 4. Use a Code Signing Certificate
Digitally signing your code using a code signing certificate will make your code tamper-proof, making it impossible for third parties to tamper with your code. A code signing certificate will make sure your files remain secure and it will also prevent hackers from adding security vulnerabilities to your code.

### Impact of Software Security Vulnerabilities


**[`^        back to top        ^`](#)**

## License
MIT License & [cc](https://creativecommons.org/licenses/by/4.0/) license

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

To the extent possible under law, [Paul Veillard](https://github.com/paulveillard/) has waived all copyright and related or neighboring rights to this work.
