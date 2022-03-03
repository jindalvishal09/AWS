[<img alt="acosalens" width="300px" src="https://github.com/jindalvishal09/AWS/blob/main/Resources/other/Acosa_logo.png" />](https://acosalens.com)

# 🎯 Managing Password Policy

## 🌐 Quick Info

### ⚡ _What is Password Policy?_

A password policy defines the password strength rules that are used to determine whether a new password is valid. A password strength rule is a rule to which a password must conform. For example, password strength rules might specify that the minimum number of characters of a password must be 5.

## ⚡ Detailed Steps

1. Log into the AWS Management Console from root user.</br></br>
2. Click on the AWS account name at the top right corner on AWS management console and click on the **"Security Credentials".**</br></br><img src="/Resources/IAM/01_Securing Root User/step_2.png"/></br></br>
3. On **"Your Security Credentials"** page scroll down and click on the **"Multi-factor authentication (MFA)"**.If the **"Activate MFA"** button is showing then a multi-factor authentication device is not enabled for the root account.Click on the "Activate MFA" button to enable a multi-factor authentication device.</br></br><img src="/Resources/IAM/01_Securing Root User/step_3.png"/></br></br>
4. Click on the **"Virtual MFA device"** and click on "Continue". </br></br><img src="/Resources/IAM/01_Securing Root User/step_4.png"/></br></br>
5. Install the AWS MFA compatible application on your mobile device or computer. Once done click on the **"Show QR code"** and scan the code with application.</br></br><img src="/Resources/IAM/01_Securing Root User/step_5.png"/></br></br>
6. Enter two consecutive MFA codes generated from application in **"MFA code 1"** and **"MFA code 2"** and click on the **"Assign MFA"** button.</br></br><img src="/Resources/IAM/01_Securing Root User/step_6.png"/></br></br>
7. On successful setup will get the following message **"You have successfully assigned virtual MFA".** </br></br><img src="/Resources/IAM/01_Securing Root User/step_7.png"/></br></br>
8. Now "Multi-factor authentication (MFA)" is enabled for the root user.</br></br><img src="/Resources/IAM/01_Securing Root User/step_8.png"/></br></br>

### ⚡ _References_

* [Password policies](https://www.ibm.com/docs/en/spim/2.0.0?topic=administration-password-policies)
