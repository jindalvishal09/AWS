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

### ⚡ _IAM is made up of_

1. **Users**- An AWS Identity and Access Management (IAM) user is an entity that you create in AWS to represent the person or application that uses it to interact with AWS. A user in AWS consists of a name and credentials.
   * _How AWS identifies an IAM user:_
	   - A "friendly name" for the user, which is the name that you specified when you created the user, such as Richard or Anaya. These are the names you see in the AWS Management Console.
	   - An Amazon Resource Name (ARN) for the user. You use the ARN when you need to uniquely identify the user across all of AWS. For example, you could use an ARN to specify the user as a Principal in an IAM policy for an Amazon S3 bucket. An ARN for an IAM user might look like the following: arn:aws:iam::account-ID-without-hyphens:user/Richard
	   - A unique identifier for the user. This ID is returned only when you use the API, Tools for Windows PowerShell, or AWS CLI to create the user; you do not see this ID in the console.
	   
2. **Users groups**-An IAM user group is a collection of IAM users. User groups let you specify permissions for multiple users, which can make it easier to manage the permissions for those users. For example, you could have a user group called Admins and give that user group typical administrator permissions. Any user in that user group automatically has Admins group permissions.

	* _Some important characteristics of user groups:_

		- A user group can contain many users, and a user can belong to multiple user groups.
		- User groups can't be nested; they can contain only users, not other user groups.
		- There is no default user group that automatically includes all users in the AWS account. If you want to have a user group like that, you must create it and assign each new user to it.
		- The number and size of IAM resources in an AWS account, such as the number of groups, and the number of groups that a user can be a member of, are limited

3. **Roles**-An IAM role is an IAM identity that you can create in your account that has specific permissions. An IAM role is similar to an IAM user, in that it is an AWS identity with permission policies that determine what the identity can and cannot do in AWS. However, instead of being uniquely associated with one person, a role is intended to be assumable by anyone who needs it. Also, a role does not have standard long-term credentials such as a password or access keys associated with it. Instead, when you assume a role, it provides you with temporary security credentials for your role session.

4. **Policies**-You manage access in AWS by creating policies and attaching them to IAM identities (users, groups of users, or roles) or AWS resources. A policy is an object in AWS that, when associated with an identity or resource, defines their permissions. AWS evaluates these policies when an IAM principal (user or role) makes a request. Permissions in the policies determine whether the request is allowed or denied. Most policies are stored in AWS as JSON documents.

### ⚡ _Security of IAM and Users in AWS_

IAM is a service provided by AWS without any cost. It's a global resilience managed service by AWS. So security of the cloud (IAM) is taken care of by AWS. Now the users within the account **users created within IAM** needs to be secured.

1. **Create admin user or users via IAM** who will act as super user of the account discounted the special powers of root user. [Click for Hands On Lab](01_Creating_adminuser_with_policy.md)
2. **Create admin user group** instead of attaching policy directly to the user create a group and attach policy to the group and add user to the group.On similar lines different groups for developer/tester/etc. can be created. [Click for Hands On Lab](02_Creating_admin_group.md). 
3. **Managing Password Policy** we can enable password policy at the account level to make passwords more compliant to best practises.
4. For rest of the users created via IAM we activate MFA and as best practise rotate access keys (if generated) periodically.

### ⚡ _IAM Account Alias_

By default the login URL for your account is **https://-accountid-.signin.aws.amazon.com/console.** This is a bit cumbersome to remember. For this you have an option to replace the account id with an alias like one for prod account and one for dev account instead of remembering the different account id's. **Keep in mind alias need to be unique globally like your account id.** You can update the alias in the IAM service as shown below.</br></br><img src="/Resources/IAM_basic/account_allias.png"/>

The sign in URL hence genereated like **https://-alias-.signin.aws.amazon.com/console.** is unique to your account. And this can be bookmarked to login via IAM user to the particular account.

### ⚡ _References_

* [IAM Official Guide](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)

* [What is IAM?](https://www.techtarget.com/searchsecurity/definition/identity-access-management-IAM-system)
