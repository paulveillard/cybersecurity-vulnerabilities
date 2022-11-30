#  Security Vulnerabilities

An ongoing & curated collection of awesome software best practices and techniques, libraries and frameworks, E-books and videos, websites, blog posts, links to github Repositories, technical guidelines and important resources about  Software Vulnerabilities in Cybersecurity.
> Thanks to all contributors, you're awesome and wouldn't be possible without you! Our goal is to build a categorized community-driven collection of very well-known resources.

![cybersecurity](https://github.com/paulveillard/cybersecurity-vulnerabilities/blob/main/Img/vulnerabilitiies.png)

## Table of Contents
- [Introduction](#)
  - [What is a Vulnerability](#)
  - [Examples of Vulnerabilities](#)
  - [List of Vulnerabilities](#)
  - [How to Prevent Software Vulnerabilities](#)
  - [Impact of Software Security Vulnerabilities](#)


## Introduction

### What is a Vulnerability?
- A vulnerability is a hole or a weakness in the application, which can be a design flaw or an implementation bug, that allows an attacker to cause harm to the stakeholders of an application. 
> Stakeholders include the application owner, application users, and other entities that rely on the application.

![threats](https://github.com/paulveillard/cybersecurity-threats/blob/main/Img/Vulnerability-Assessment-Idenitfying-Vulnerabilities.jpg)

### Examples of Vulnerabilities

- Lack of input validation on user input
- Lack of sufficient logging mechanism
- Fail-open error handling
- Not closing the database connection properly

### List of Vulnerabilities

##### Allowing Domains or Accounts to Expire

##### Buffer Overflow
- Buffer overflow occurs when an attempt is made to store data that is too big for the memory space allocated. Attackers can use this software coding mistake, where the storage capacity of a program is overwritten, to take control of or to access your system. This vulnerability tends to be more common in software written in C and C++. Many programming languages have automatic protection against buffer overflow attacks.

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
