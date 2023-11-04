<h1>Changing file permissions in Linux</h1>

<h2>Description</h2>
This was an instance where I was practicing changing file and directory permissions in Linux via a lab.
<br />

<h2>Environments Used </h2>

- <b>iPadOS</b>

<h2>Program walkthrough:</h2>

<p align="center">
First I'll check file and directory details. pwd allows you to see which directory you're in and ls -la allows you to check permissions for all files and directories, including hidden files: <br/>
<a href="https://imgur.com/Xb0BopE"><img src="https://i.imgur.com/Xb0BopE.png" title="source: imgur.com" /></a>
<br />
<br />
To understand the 10 character string on the left, d indicates a directory and - indicates a regular file. The next three characters after that indicate the user and which permissions they have. The three after that is the group and the three after that is other. r indicates permission to read, w indicates the permission to write and x indicates permission to execute. For this exercise, I don't want others to have write permission for the project_k.txt file so I'm going to revoke their permission.
<p align="center">
Revoking others' write permission for project_k.txt so that they could only read the file. :  <br/>
<a href="https://imgur.com/0aff5Nh"><img src="https://i.imgur.com/0aff5Nh.png" title="source: imgur.com" /></a>
Afterwards I used ls -la again to confirm that the changes were made. chmod allows me to change permissions. The command o-w indicates that I am revoking write permission for other. Next I want to revoke the group's read permission for project_m.txt so that only the user can read and write.
<p align="center">
Revoking the group's read permission for project_m.txt:  <br/>
<a href="https://imgur.com/G63yTEZ"><img src="https://i.imgur.com/G63yTEZ.png" title="source: imgur.com" /></a>
Again, confirming afterwards that the changes were made. For the next step, I don't want the user or the group to have write permission for the .project_x.txt hidden file. You know it's a hidden file because it has a . before the name.
<p align="center">
Revoking the user and the group's write permissions for the .project_x.txt hidden file:  <br/>
<a href="https://imgur.com/xxsoeQO"><img src="https://i.imgur.com/xxsoeQO.png" title="source: imgur.com" /></a>
Finally, after clearing everything to clean up the screen using the clear command, I navigated to the drafts directory using the cd command. I don't want the group to have execute permission for this directory so I'm going to revoke their permission:  <br/>
<p align="center">
Revoking the group's execute permission for the drafts directory:  <br/>
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
