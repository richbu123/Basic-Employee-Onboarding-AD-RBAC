# Basic Employee Onboarding (AD)(RBAC)

## Problem Statement
Northstar Medical Group (NMG) relied on an MSP to handle the user lifecycle and access management. However, due to mismanagement on the MSP's part, user creation was manual and could take days as no one internally knew the process. There were no Organizational Units (OUs) in the Active Directory (AD) and the user rights assignment was inconsistent leading to elevated privileges for some users. This poses a huge risk to NMGs HIPAA compliance which NMG cannot have happen.

## Solution Overview
I built a server on a VM to server as NMGs new Domain Controller (DC). This DC serves as the basis of identity authentication in the environment; Each sign in goes back to the Domain Controller to ask if this person exists in the environment and what should they be able to access along with what their experience in the environment should be. Next was the OUs and the security groups. These combined allows for Role Based Access (RBAC) where we can assign certain privileges based on what a user does for their job. OUs and Security Groups were made for each department and users were added for proper management. This is better than the old model as there is consistent access management which lessens the possibilities of breaches due to Broken Access Management. 

## Video Walkthrough
[Walkthrough](https://www.loom.com/share/b3176eebff764f718736a007a3cd6866)

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* RBAC
* GitHub

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* Built documentation for my project and a ticket resolution
* Got more comfortable with troubleshooting VMs
