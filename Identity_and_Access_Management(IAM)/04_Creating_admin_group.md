[<img alt="acosalens" width="300px" src="https://github.com/jindalvishal09/AWS/blob/main/Resources/other/Acosa_logo.png" />](https://acosalens.com)

# 🎯 Creating Admin Group

## 🌐 Quick Info

### ⚡ _Why to create Groups?_

An IAM user group is a collection of IAM users. User groups let you specify permissions for multiple users, which can make it easier to manage the permissions for those users. For example, you could have a user group called Admins and give that user group typical administrator permissions. Any user in that user group automatically has Admins group permissions. If a new user joins your organization and needs administrator privileges you can assign the appropriate permissions by adding the user to the Admins user group.
</br></br><img src="/Resources/admin_user/groups.png"/></br></br>

## ⚡ Detailed Steps

1. Log into the AWS Management Console from root user.</br></br>
2. Search IAM in the search bar at top of console and then click **"IAM".** This will take you to IAM dashboard.</br></br><img src="/Resources/admin_user/IAM_Service_Search.png"/></br></br>
3. On **"IAM dashboard's"** left panel click **User groups.**</br></br><img src="/Resources/admin_user/user_groups.png"/></br></br>
4. Click **Create Group**. </br></br><img src="/Resources/admin_user/create_group.png"/></br></br>
5. Name the group as **admins** and select the **iamadmin** user to be part of this group.</br></br><img src="/Resources/admin_user/group_name.png"/></br></br>
  * Scroll down to **Attach permissions policies** and type  **AdministratorAccess** in search feild and click enter. Select **AdministratorAccess** policy and Click **Create Group**</br></br><img src="/Resources/admin_user/policy_attach.png"/></br></br>
7. User group created message will be displayed.</br></br><img src="/Resources/admin_user/group_success.png"/></br></br>

### Detaching Policy from the user
---
As the admin policy is now attached to the user via group we need to remove the policy from the admin user **IAMADMIN**

1. On **"IAM dashboard's"** left panel click **Users.**</br></br><img src="/Resources/admin_user/users_panel.png"/></br></br>
2. Click on **IAMADMIN USER** </br></br><img src="/Resources/admin_user/user_iamadmin.png"/></br></br>
3. Under **Attached directly** click the **cross** symbol in front of **AdministratorAccess** </br></br><img src="/Resources/admin_user/remove_policy.png"/></br></br>
4. Click on **Detach** to confirm the action </br></br><img src="/Resources/admin_user/detach_confirmation.png"/></br></br>
5. After screen refresh the **Attached directly** section will be removed.
