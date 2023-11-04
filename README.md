<h1>Changing file permissions in Linux</h1>

<h2>Description</h2>
This was an instance where I was practicing changing file and directory permissions in Linux via a lab.
<br />

<h2>Environments Used </h2>

- <b>iPadOS</b>

<h2>Program walkthrough:</h2>

<p align="center">
Checking file and directory details: <br/>
<a href="https://imgur.com/Xb0BopE"><img src="https://i.imgur.com/Xb0BopE.png" title="source: imgur.com" /></a>
<br />
<br />
Revoking others' write permission for project_k.txt so that they could only read the file:  <br/>
<a href="https://imgur.com/0aff5Nh"><img src="https://i.imgur.com/0aff5Nh.png" title="source: imgur.com" /></a>
Next I revoked the group's read permission for project_m.txt so that only the user could read and write:  <br/>
<a href="https://imgur.com/G63yTEZ"><img src="https://i.imgur.com/G63yTEZ.png" title="source: imgur.com" /></a>
Now I revoked the user's and the group's write permissions for the .project_x.txt hidden file:  <br/>
<a href="https://imgur.com/xxsoeQO"><img src="https://i.imgur.com/xxsoeQO.png" title="source: imgur.com" /></a>
Finally, after clearing everything to clean up the screen, I navigated to the drafts directory and revoked the group's execute permission for the drafts directory:  <br/>
<a href="https://imgur.com/t2noJdt"><img src="https://i.imgur.com/t2noJdt.png" title="source: imgur.com" /></a>

<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
