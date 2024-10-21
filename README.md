<h1>Botium Toys: Scope, goals, and risk assessment </h1>


<h2>Description</h2>
This project details an internal security audit I conducted for a fictitious company and scenario. Audits help ensure that security checks are made, to monitor for threats, risks, or vulnerabilities that can affect an organization’s business continuity and critical assets. <br/><br/>
The NIST CSF groups cybersecurity processes and activities into 5 high-level categories (functions) that can aid organizations in creating a structured approach for securing IT systems. The categories are <b>identify, protect, detect, respond and recover</b>. NIST further defines 8 cyber resilience objectives that can be attributed to these categories. These objectives can be achieved using various techniques.<br/><br/>
<b>Project Scenario: </b><br/>
<i>Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location, which serves as their main office, a storefront, and warehouse for their products. However, Botium Toy’s online presence has grown, attracting customers in the U.S. and abroad. As a result, their information technology (IT) department is under increasing pressure to support their online market worldwide. <br/><br/>

The manager of the IT department has decided that an internal IT audit needs to be conducted. She's worried about maintaining compliance and business operations as the company grows without a clear plan. She believes an internal audit can help better secure the company’s infrastructure and help them identify and mitigate potential risks, threats, or vulnerabilities to critical assets. The manager is also interested in ensuring that they comply with regulations related to internally processing and accepting online payments and conducting business in the European Union (E.U.). <br/><br/>

The IT manager starts by implementing the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF), establishing an audit scope and goals, listing assets currently managed by the IT department, and completing a risk assessment. The goal of the audit is to provide an overview of the risks and/or fines that the company might experience due to the current state of their security posture.</i><br />


<h2>Languages and Utilities Used</h2>

- <b>None</b> 

<h2>Environments Used </h2>

- <b>None</b>

<h2>Program walk-through:</h2>

<p align="center">
  <b>Scope and goals of the audit</b></p>  <br/>
  
<b>Scope: </b><br/>

The scope of this audit is defined as the entire security program at Botium Toys. This includes their assets like employee equipment and devices, their internal network, and their systems. You will need to review the assets Botium Toys has and the controls and compliance practices they have in place.
<br /><br/>
<b>Goals: </b><br/>

Assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices that need to be implemented to  improve Botium Toys’ security posture.
<br />
<img src="http://i.imghippo.com/files/JUl8767ro.png" height="80%" width="80%" alt=""/>
<br />


<!--<p align="center">--!><b>1. Understand the Context, IT Systems Criticality and Risk Factors (Identify)</b>  <br/></p>
The 10-character string can be deconstructed to determine who is authorized to access the file and their specific permissions. The characters and what they represent are as follows:<br/>
- 1st character: This character is either a d or hyphen (-) and indicates the file type. If it’s a d, it’s a directory. If it’s a hyphen (-), it’s a regular file.<br/>
- 2nd-4th characters: These characters indicate the read (r), write (w), and execute (x) permissions for the user. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted to the user.<br/>
- 5th-7th characters: These characters indicate the read (r), write (w), and execute (x) permissions for the group. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted for the group.<br/>
- 8th-10th characters: These characters indicate the read (r), write (w), and execute (x) permissions for other. This owner type consists of all other users on the system apart from the user and the group. When one of these characters is a hyphen (-) instead, that indicates that this permission is not granted for other.
<br />
<br />
<p align="center">
  <b>Change File Permissions</b></p>  <br/>
The organization determined that other shouldn't have write access to any of their files. To comply with this, I referred to the file permissions that I previously returned. I determined project_k.txt must have the write access removed for other.<br/>
<br/>

The following code demonstrates how I used Linux commands to do this:<br/>

<img src="https://i.imghippo.com/files/iVsmE1729471023.png" height="80%" width="80%" alt=""/>

The first two lines of the screenshot display the commands I entered, and the other lines display the output of the second command. The chmod command changes the permissions on files and directories. The first argument indicates what permissions should be changed, and the second argument specifies the file or directory. In this example, I removed write permissions from other for the project_k.txt file. After this, I used ls -la to review the updates I made.<br/>
<br/>

<p align="center">
  <b>Change file permissions on a hidden file</b></p>  <br/>
The research team at my organization recently archived project_x.txt. They do not want anyone to have write access to this project, but the user and group should have read access. <br/>
<br/<

The following code demonstrates how I used Linux commands to change the permissions:<br/>

<img src="https://i.imghippo.com/files/ImMnT1729471344.png" height="80%" width="80%" alt=""/>
The first two lines of the screenshot display the commands I entered, and the other lines display the output of the second command. I know .project_x.txt is a hidden file because it starts with a period (.). In this example, I removed write permissions from the user and group, and added read permissions to the group. I removed write permissions from the user with u-w. Then, I removed write permissions from the group with g-w, and added read permissions to the group with g+r. 
<br />
<br />
<p align="center">
  <b>Change directory permissions</b></p>  <br/>
My organization only wants the researcher2 user to have access to the drafts directory and its contents. This means that no one other than researcher2 should have execute permissions.<br/>
<br/>
The following code demonstrates how I used Linux commands to change the permissions:<br/>

<img src="https://i.imghippo.com/files/paBbB1729471466.png" height="80%" width="80%" alt=""/>
The output here displays the permission listing for several files and directories. Line 1 indicates the current directory (projects), and line 2 indicates the parent directory (home). Line 3 indicates a regular file titled .project_x.txt. Line 4 is the directory (drafts) with restricted permissions. Here you can see that only researcher2 has execute permissions.  It was previously determined that the group had execute permissions, so I used the chmod command to remove them. The researcher2 user already had execute permissions, so they did not need to be added.
<br />
<br />
<p align="center">
  <b>Summary</b></p>  <br/>

I changed multiple permissions to match the level of authorization my organization wanted for files and directories in the projects directory. The first step in this was using ls -la to check the permissions for the directory. This informed my decisions in the following steps. I then used the chmod command multiple times to change the permissions on files and directories.

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

