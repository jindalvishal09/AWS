[<img alt="acosalens" width="300px" src="https://github.com/jindalvishal09/AWS/blob/main/Resources/other/Acosa_logo.png" />](https://acosalens.com)

# 🎯 Creating Admin User- With attached policy

## 🌐 Quick Info

### ⚡ _Why to create Admin User/Users?_

Root user is the only user in your AWS account which is unristricted and also can't be restricted as it is the super user of your account. So to do all admin work without the Root user
we need admin user or users to perfom admin task.

## ⚡ Detailed Steps

1. Log into the AWS Management Console from root user.</br></br>
2. Search IAM in the search bar at top of console and then click **"IAM".** This will take you to IAM dashboard.</br></br><img src="/Resources/admin_user/IAM_Service_Search.png"/></br></br>
3. On **"IAM dashboard's"** left panel click **Users.**</br></br><img src="/Resources/admin_user/users_panel.png"/></br></br>
4. Click **Add users**. </br></br><img src="/Resources/admin_user/add_users.png"/></br></br>
5. Fill up the details as needed on the adduser page.</br></br><img src="/Resources/admin_user/add_user_1.png"/></br></br>
  * If you decide to choose **AWS Management Console access** as an option, you need to select few more options as below. Click **Next: Permissions**</br></br><img src="/Resources/admin_user/password_option.png"/></br></br>
7. You need to provide **Permissions** to the user. Here we are giving direct permission via AWS managed admin policy. Click **Next: Tags**</br></br><img src="/Resources/admin_user/user_permission.png"/></br></br>
8. You can add **Tags- optional(Key value pair)** to tag metadata for this user such as department.Click **Next: Review**</br></br><img src="/Resources/admin_user/user_tags.png"/></br></br>
9. Review details provided till now and Click **Create User**</br></br><img src="/Resources/admin_user/review.png"/></br></br>
10. You will see a **Success** message providing the details of user created</br></br><img src="/Resources/admin_user/success.png"/></br></br>
