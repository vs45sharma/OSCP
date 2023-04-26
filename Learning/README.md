1.[CTFtime.org](https://ctftime.org/writeups)

2.[Hackthebox](https://app.hackthebox.com/home)

3.[Hackthebox Academy](https://academy.hackthebox.com/dashboard)

4.[TryHackMe](https://tryhackme.com/)

5.[PortSwigger](https://portswigger.net/web-security)

6.[Offensive-Security](https://portal.offensive-security.com/labs/play)

7.[HackerOne](https://www.hacker101.com/)

8.[vulnmachines](https://account.vulnmachines.com/user/challenges)


```css
DLL Hijacking

https://github.com/wietze/HijackLibs

https://hijacklibs.net/
```
Blogs
```
https://securiumsolutions.com/blog/
https://www.cobalt.io/
https://blog.rehack.xyz/
```

https://infosecwriteups.com/how-i-found-3-bug-bounties-in-a-day-c82fe023716e

https://infosecwriteups.com/detecting-log4j-its-remediation-58ab3a59c865

https://infosecwriteups.com/how-to-perform-command-injection-attacks-dvwa-for-aspiring-hackers-stackzero-c9d521c6f934

```
Web Application 
https://github.com/OWASP/wstg/tree/master/document/4-Web_Application_Security_Testing

Flaw 	Real-world Scenario
SQL injection :-
Obtaining Active Directory usernames and performing a password spraying attack against a VPN or email portal.

File Inclusion :-
Reading source code to find a hidden page or directory which exposes additional functionality that can be used to gain remote code execution.

Unrestricted File Upload :-	
A web application that allows a user to upload a profile picture that allows any file type to be uploaded (not just images). This can be leveraged to gain full control of the web application server by uploading malicious code.

Insecure Direct Object Referencing (IDOR) :-
When combined with a flaw such as broken access control, this can often be used to access another user's files or functionality. An example would be editing your user profile browsing to a page such as /user/701/edit-profile. If we can change the 701 to 702, we may edit another user's profile!

Broken Access Control :-
Another example is an application that allows a user to register a new account. If the account registration functionality is designed poorly, a user may perform privilege escalation when registering. Consider the POST request when registering a new user, which submits the data username=bjones&password=Welcome1&email=bjones@inlanefreight.local&roleid=3. What if we can manipulate the roleid parameter and change it to 0 or 1. We have seen real-world applications where this was the case, and it was possible to quickly register an admin user and access many unintended features of the web application.
```

https://github.com/debug601/bug_report/tree/main/vendors/kingbhob02/library-management-system
