[<img alt="acosalens" width="300px" src="https://github.com/jindalvishal09/AWS/blob/main/Resources/other/Acosa_logo.png" />](https://acosalens.com)

# Basics of AWS account

### ⚡ _What is Account?_
An AWS account is a container for your AWS resources. You create and manage your AWS resources in an AWS account, and the AWS account provides administrative capabilities for access and billing.

### ⚡ _Basic components of Account_

While creating an account you need to provide a unique **email address**, a account name **like Developement/Prod/Test** and **credit card information** for biiling purpose.

Credentials **(email address and password)** which you used to create an account is used to create a user called as **Root User** of your account. It has full access to you account and this user can't be restricted.

All the resources consumed with the AWS account is billed against the account payment method i.e. **credit card** used for account creation.

Using multiple AWS accounts is a best practice for scaling your environment, as it provides a natural billing boundary for costs, isolates resources for security, gives flexibility or individuals and teams, in addition to being adaptable for new business processes.

AWS account uses a concept called as **Principle of Least Privilege** which means a subject should be given only those privileges needed for it to complete its task. Hence
by default all access to an AWS account and resources is denied by default except for **root user**.

### ⚡ _References_

* [AWS Organizations FAQs](https://aws.amazon.com/organizations/faqs/)
