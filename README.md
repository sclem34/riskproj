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
I first needed to understand the context, IT systems, and risk levels of the business. <br/><br/>
<b>Risk description</b><br/>
Currently, assets are being managed inadequately. Additionally, Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations and standards.  <br/>
<br/>
<b>Control best practices</b><br/>
The first of the five functions of the NIST CSF is Identify. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they will need to classify existing assets and determine the impact of the loss of existing assets, including systems, on business continuity.<br/><br/>
<b>Risk score</b><br/>
On a scale of 1 to 10, the risk score is 8, which is fairly high. This is due to a lack of controls and adherence to compliance best practices.<br/>
by completing a controls and compliance checklist found in my files.

<br />
<br />
<p align="center">
  <b>Assessment Summary</b></p>  <br/>

The potential impact from the loss of an asset is rated as medium, because the IT department does not know which assets would be at risk. The risk to assets or fines from governing bodies is high because Botium Toys does not have all of the necessary controls in place and is not fully adhering to best practices related to compliance regulations that keep critical data private/secure. Review the following bullet points for specific details:<br/><br/>
- Currently, all Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII.<br/>
- Encryption is not currently used to ensure confidentiality of customers’ credit card information that is accepted, processed, transmitted, and stored locally in the company’s internal database. <br/>
- Access controls pertaining to least privilege and separation of duties have not been implemented.<br/>
- The IT department has ensured availability and integrated controls to ensure data integrity.<br/>
- The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules.<br/>
- Antivirus software is installed and monitored regularly by the IT department. <br/>
- The IT department has not installed an intrusion detection system (IDS).<br/>
- There are no disaster recovery plans currently in place, and the company does not have backups of critical data.<br/> 
- The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach. Additionally, privacy policies, procedures, and processes have been developed and are enforced among IT department members/other employees, to properly document and maintain data.<br/>
- Although a password policy exists, its requirements are nominal and not in line with current minimum password complexity requirements (e.g., at least eight characters, a combination of letters and at least one number; special characters). <br/>
- There is no centralized password management system that enforces the password policy’s minimum requirements, which sometimes affects productivity when employees/vendors submit a ticket to the IT department to recover or reset a password.<br/>
- While legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear.<br/>
- The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has sufficient locks, up-to-date closed-circuit television (CCTV) surveillance, as well as functioning fire detection and prevention systems.
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

