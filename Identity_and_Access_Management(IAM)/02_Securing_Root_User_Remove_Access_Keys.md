[<img alt="acosalens" width="300px" src="https://github.com/jindalvishal09/AWS/blob/main/Resources/other/Acosa_logo.png" />](https://acosalens.com)

# 🎯 Securing Root User-Removing Access Keys

## 🌐 Quick Info

### ⚡ _Why to secure a Root User?_

Root user is the only user in your AWS account which is unristricted and also can't be restricted as it is the super user of your account. In case your usrname/password get's compromised you will loose the complete control of your AWS account. So you need to 
1. Enable MFA [Link to Lab](https://github.com/jindalvishal09/AWS/blob/main/Identity_and_Access_Management(IAM)/01_Securing_Root_User_MFA.md)
2. Delete all access keys for root user to disable programmatic  access from root user.

### ⚡ _What are access keys_

Access keys are long-term credentials for an IAM user or the AWS account root user. You can use access keys to sign programmatic requests to the AWS CLI or AWS API (directly or using the AWS SDK).
Access keys consist of two parts: an access key ID (for example, AKIAIOSFODNN7EXAMPLE) and a secret access key (for example, wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY). Like a user name and password, you must use both the access key ID and secret access key together to authenticate your requests. Manage your access keys as securely as you do your user name and password.

## ⚡ Detailed Steps

1. Log into the AWS Management Console from root user.</br></br>
2. Click on the AWS account name at the top right corner on AWS management console and click on the **"Security Credentials".**</br></br><img src="/Resources/IAM/01_Securing Root User/step_2.png"/></br></br>
3. On **"Your Security Credentials"** page scroll down and click on the **"Access keys (access key ID and secret access key)"**.If there are any keys created already that will be shown here</br></br><img src="/Resources/IAM/01_Securing Root User/step_9.png"/></br></br>
4. If there are keys,click on the **"Delete"** against the key to be deleted. </br></br><img src="/Resources/IAM/01_Securing Root User/step_10.png"/></br></br>
5. You first need to **Deactivate the key**.</br></br><img src="/Resources/IAM/01_Securing Root User/step_11.png"/></br></br>
6. Manually type in the key value in the text field to confirm the deletion and click **Delete**</br></br><img src="/Resources/IAM/01_Securing Root User/step_12.png"/></br></br>
7. On successful deletion you will get ststus as deleted against the key </br></br><img src="/Resources/IAM/01_Securing Root User/step_13.png"/></br></br>
