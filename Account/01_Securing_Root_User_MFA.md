[<img alt="acosalens" width="300px" src="https://github.com/jindalvishal09/AWS/blob/main/Resources/other/Acosa_logo.png" />](https://acosalens.com)

# 🎯 Securing Root User-MFA

## 🌐 Quick Info

### ⚡ _Why to secure a Root User?_

Root user is the only user in your AWS account which is unristricted and also can't be restricted as it is the super user of your account. In case your usrname/password get's compromised you will loose the complete control of your AWS account. So you need to 
1. Enable MFA
2. Delete all access keys for root user to disable programmatic access from root user.[Link to Lab](https://github.com/jindalvishal09/AWS/blob/main/Identity_and_Access_Management(IAM)/02_Securing_Root_User_Remove_Access_Keys.md)

### ⚡ _What is an Authentication Factor?_

An authentication factor is a special category of security credential that is used to verify the identity and authorization of a user attempting to gain access, send communications, or request data.

### ⚡ _Five Authentication Factor Categories and How They Work_

1. **Knowledge Factors** :- Knowledge factors require the user to provide some data or information before they can access a secured system. a password or personal identification number (PIN).
2. **Possession Factors** :- Possession factors require the user to possess a specific piece of information or device before they can be granted access to the system.Like credit card, MFA Device
3. **Inherence Factors** :- Inherence factors authenticate access credentials based on factors that are unique to the user. These include fingerprints, thumbprints, and palm or handprints.
4. **Location Factors** :- Network administrators can implement services that use geolocation security checks to verify the location of a user before granting access to an application, network or system
5. **Behavior Factors** :- A behavior-based authentication factor is based on actions undertaken by the user to gain access to the system.Mobile phone lock-screens where the user is required to draw a specific pattern onto a grid of dots



## ⚡ Detailed Steps

1. Log into the AWS Management Console from root user.</br></br>
2. Click on the AWS account name at the top right corner on AWS management console and click on the **"Security Credentials".**</br></br><img src="/Resources/IAM/01_Securing Root User/step_2.png"/></br></br>
3. On **"Your Security Credentials"** page scroll down and click on the **"Multi-factor authentication (MFA)"**.If the **"Activate MFA"** button is showing then a multi-factor authentication device is not enabled for the root account.Click on the "Activate MFA" button to enable a multi-factor authentication device.</br></br><img src="/Resources/IAM/01_Securing Root User/step_3.png"/></br></br>
4. Click on the **"Virtual MFA device"** and click on "Continue". </br></br><img src="/Resources/IAM/01_Securing Root User/step_4.png"/></br></br>
5. Install the AWS MFA compatible application on your mobile device or computer. Once done click on the **"Show QR code"** and scan the code with application.</br></br><img src="/Resources/IAM/01_Securing Root User/step_5.png"/></br></br>
6. Enter two consecutive MFA codes generated from application in **"MFA code 1"** and **"MFA code 2"** and click on the **"Assign MFA"** button.</br></br><img src="/Resources/IAM/01_Securing Root User/step_6.png"/></br></br>
7. On successful setup will get the following message **"You have successfully assigned virtual MFA".** </br></br><img src="/Resources/IAM/01_Securing Root User/step_7.png"/></br></br>
8. Now "Multi-factor authentication (MFA)" is enabled for the root user.</br></br><img src="/Resources/IAM/01_Securing Root User/step_8.png"/></br></br>


[Reference](https://www.sumologic.com/glossary/authentication-factor/)
