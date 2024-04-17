<h1>Detecting Web Attacks</h1>

<h2>Description</h2>
Investigate Multiple Suspected Web Attacks by Searching Web Server Access Logs for Evidence of Common Attacks. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Sublime Text Editor</b>
- <b>Web Server Access Logs</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>

<br />

<h2>Analysis:</h2>

<p align="center">
Example 1: <br/>
<img src="https://i.imgur.com/tqLWapQ.png" height="80%" width="80%" alt="Web Attacks "/>
<br />

Beginning at line 145, evidence suggests an SQL injection attack originating from IP address 192.168.31.167. This is indicated by the presence of common SQL terms such as 'UNION' and 'SELECT.' Regrettably, the attack seems to have succeeded, as evidenced by the successful HTTP response status code and a noticeable increase in response size.
<br />

<p align="center">
Example 2: <br/>
<img src="https://i.imgur.com/iUPNSyn.png" height="80%" width="80%" alt="Web Attacks "/>
<br />

Starting at line 213, there are indications of a command injection attack from IP address 192.168.31.156. This is evident from the presence of common Linux CLI commands such as 'ls,' 'whoami,' 'dir,' and 'pwd.' Despite encountering successful HTTP response status codes, there was no change in response size, suggesting the attempt was unsuccessful.
<br />

<p align="center">
Example 3: <br/>
<img src="https://i.imgur.com/xbSnCqP.png" height="80%" width="80%" alt="Web Attacks "/>
<br />

Beginning at line 178, there are signs of a file inclusion attack originating from IP address 192.168.31.174. This is evident from the presence of multiple '../' sequences followed by a file path, a common technique used by attackers to navigate the file system. Despite encountering successful HTTP response status codes, the lack of change in response size suggests the attack was unsuccessful.
<br />

<p align="center">
Example 4: <br/>
<img src="https://i.imgur.com/7VJEHcs.png" height="80%" width="80%" alt="Web Attacks "/>
<br />

Starting at line 226, there are signs of an IDOR attack originating from IP address 192.168.31.174. This is evidenced by multiple requests for the same page, each with changing 'id' parameters. The successful HTTP response status code and the observed change in response size suggest that this attack was indeed successful.
<br />

<p align="center">
Example 5: <br/>
<img src="https://i.imgur.com/VJydrRF.png" height="80%" width="80%" alt="Web Attacks "/>
<br />

Beginning at line 185, there are indications of a Cross-Site Scripting (XSS) attack originating from IP address 192.168.31.183. This is evident from injected code within the 'name' field on the website. The presence of a successful HTTP response status code and the observed change in response size suggest that this attack has indeed been successful.
<br />

<h2>Conclusion</h2>
It's evident that sanitizing user input is crucial to prevent many of these common attacks and should be a fundamental part of secure coding practices. This measure should encompass not only form data but also URL parameters, headers, and any other form of user input.
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
