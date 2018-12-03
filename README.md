# Week8CP
# Project 8 - Pentesting Live Targets

Time spent: **20** hours spent in total

## Pentesting Report

1. (Required) Cross-site scripting (GREEN1)
  - [ ] Summary: Simple attack on a web site
    - Vulnerability types: Cross-site scripting
  - [GIF]GIF Walkthrough: [Link](https://media.giphy.com/media/1qZ91rSfvF3a3sFgGT/giphy.gif)
  - [ ] Steps to recreate: 
  Throguh the contact form before you log in, you can sned a feedback with your name, email and comment. Put a malcious comment and log into the web site, and then open the feedback and you will see the thing.
  - [ ] Affected source code:
    - [Link 1](https://104.198.208.81/green/public/staff/feedback/index.php)
    
    
2. (Required) User Enumeration (BLUE1)
  - [ ] Summary: Get lists of users.
    - Vulnerability types: SQLI
  - [ ]() GIF Walkthrough: 
  - [ ] Steps to recreate: Go to a page showing some users and manipulate the URL so taht it shows id=' OR 1=1 --' at the end of it.
  - [ ] Affected source code:
    - [Link 1](https://104.198.208.81/blue/public/staff/salespeople/show.php?id=' OR 1=1 --')
    
    
3. (Required)Cross site request forgery (RED1)
  - [ ] Summary: The admin account can encode a malcious code on any of first name, last name, phone, or email address section, and it can jump to a bad web site. 
    - Vulnerability types:CSRF
    - Tested in version:4.2
  - [ ] GIF Walkthrough: 
  - [GIF] (https://media.giphy.com/media/39m1OPipcCwRMypJJw/giphy.gif)
  - [ ] Steps to recreate: Log in to the site, add a new person, and encode a malcious code when editing the new account. 

4. (Required) Insecure direct object reference (RED2)
  - [ ] Summary: This vulnerability is that shows an account which sould not be seen in the public.
    - Vulnerability types:IDOR
  - [ ] GIF Walkthrough: (https://media.giphy.com/media/82RIDxggtt8BxFvW17/giphy.gif)
  - [ ] Steps to recreate: Log in and out the site to check who is and is not public yet. There are some acccounts that sould not be seen in the public. So, get the ID# of one of the accounts and log out the site. Then go to the salesperson list and open a random one and change its ID# to the one that you checked and was not public. 

5. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

FireFox (Developper ver.)
Kali Linux

## Resources
- [Friend](https://github.com/FriendComp/codepathfall2018week8/blob/master/README.md)
- [Cross-site Scripting (XSS)](https://www.owasp.org/index.php/Cross-site_Scripting_(XSS))
- [The Cross-site Scripting (XSS) Vulnerability: Definition and Prevention](https://www.netsparker.com/blog/web-security/cross-site-scripting-xss/)

## Notes



## License

    Copyright [2018] [Kato 590]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
