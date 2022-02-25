[<img alt="acosalens" width="300px" src="https://github.com/jindalvishal09/AWS/blob/main/Resources/other/Acosa_logo.png" />](https://acosalens.com)

# Basics of Identity and Access Management

### ⚡ _What is identity and access management?_
Identity and access management (IAM) is a framework of business processes, policies and technologies that facilitates the management of electronic or digital identities. With an IAM framework in place, information technology (IT) managers can control user access to critical information within their organizations. Systems used for IAM include single sign-on systems, two-factor authentication, multifactor authentication and privileged access management. These technologies also provide the ability to securely store identity and profile data as well as data governance functions to ensure that only data that is necessary and relevant is shared.
On a fundamental level, IAM encompasses the following components:

1. How individuals are identified in a system (understand the difference between identity management and authentication)
2. How roles are identified in a system and how they are assigned to individuals
3. Adding, removing and updating individuals and their roles in a system
4. Assigning levels of access to individuals or groups of individuals and
5. Protecting the sensitive data within the system and securing the system itself

### ⚡ _Basic components of IAM_

An IAM framework enables IT to control user access to critical information within their organizations. IAM products offer role-based access control, which lets system administrators regulate access to systems or networks based on the roles of individual users within the enterprise.
In this context, access is the ability of an individual user to perform a specific task, such as view, create or modify a file. Roles are defined according to job, authority and responsibility within the enterprise.

IAM systems should do the following: capture and record user login information, manage the enterprise database of user identities, and orchestrate the assignment and removal of access privileges.
That means systems used for IAM should provide a centralized directory service with oversight and visibility into all aspects of the company user base.Digital identities are not just for humans; IAM can manage the digital identities of devices and applications to help establish trust.

### ⚡ _What AWS IAM Service Do?_

IAM performs 3 operations in general:
1. Manages Identity (An Identity Provider) : An identity provider (IdP) is a service that stores and manages digital identities. Helps in creating identities like Users/Groups
2. Authenticate : Verifying the identity of a user, process, or device, often as a prerequisite to allowing access to resources in an information system. The created users are authenticated by system based on Username/Password/MFA
3. Authorize: Authorization is permitting an authenticated user the permission to perform a given action on specific resources. Based on permissions and policy assigned to a group or user, actions are allowed or denied.

### ⚡ _IAM Service in AWS?_

IAM service and Root user are the only two ways to access an AWS account as your account trusts IAM- a service and Root- a user completely. And Root being the super user has more power compared to IAM service. There are certain tasks which can be done only by Root user namely:</br><img src="/Resources/IAM_basic/basic_1.png"/>
1. **Change your account settings**: This includes the account name, email address, root user password, and root user access keys. Other account settings, such as contact information, payment currency preference, and AWS Regions, don't require root user credentials.
2. **Restore IAM user permissions**: If the only IAM administrator accidentally revokes their own permissions, you can sign in as the root user to edit policies and restore those permissions.
3. **Activate IAM access to the Billing and Cost Management console.**
4. **View certain tax invoices**: An IAM user with the aws-portal:ViewBilling permission can view and download VAT invoices from AWS Europe, but not AWS Inc. or Amazon Internet Services Private Limited (AISPL).
5. **Close your AWS account.**
6. **Change your AWS Support plan or Cancel your AWS Support plan.**
7. **Register as a seller in the Reserved Instance Marketplace.**
8. **Configure an Amazon S3 bucket to enable MFA (multi-factor authentication).**
9. **Edit or delete an Amazon Simple Storage Service (Amazon S3) bucket policy that includes an invalid virtual private cloud (VPC) ID or VPC endpoint ID.**
10. **Sign up for GovCloud.**

[Reference](https://www.techtarget.com/searchsecurity/definition/identity-access-management-IAM-system)
