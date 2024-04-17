<h1>Detecting Web Attacks</h1>

<h2>Description</h2>
Investigate Multiple Suspected Web Attacks by Searching Web Server Access Logs for Common Attacks. 
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
Example 2: <br/>
<img src="https://i.imgur.com/iUPNSyn.png" height="80%" width="80%" alt="Web Attacks "/>
<br />

Starting at line 213, there are indications of a command injection attack from IP address 192.168.31.156. This is evident from the presence of common Linux CLI commands such as 'ls,' 'whoami,' 'dir,' and 'pwd.' Despite encountering successful HTTP response status codes, there was no change in response size, suggesting the attempt was unsuccessful.
<br />
<p align="center">
Example 2: <br/>
<img src="https://i.imgur.com/iUPNSyn.png" height="80%" width="80%" alt="Web Attacks "/>
<br />

Starting at line 213, there are indications of a command injection attack from IP address 192.168.31.156. This is evident from the presence of common Linux CLI commands such as 'ls,' 'whoami,' 'dir,' and 'pwd.' Despite encountering successful HTTP response status codes, there was no change in response size, suggesting the attempt was unsuccessful.
<br />

<h2>Final Report</h2>
After thorough investigation, it is evident that this email constitutes a phishing attempt. There is no indication that it was sent by PayPal, and the included links have been identified as known phishing attempts. Therefore, I recommend deleting this email immediately and performing remediation if any client has visited the URL link.
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
