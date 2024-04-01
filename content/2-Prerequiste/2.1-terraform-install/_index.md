---
title : "Install Terraform"
date :  "`r Sys.Date()`" 
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

#### Install Terraform

**Step 1**: Download Terraform
Access the official website of Terraform [here](https://developer.hashicorp.com/terraform)
Then click on "install," choose the version suitable for your operating system. For Windows, there are two versions available: 386 and AMD64. Select one of the two..
![Downloadsite](/images/2.1-terraform-install/00007.png?featherlight=false&width=70pc)
![OS](/images/2.1-terraform-install/00008.png?featherlight=false&width=70pc)

**Step 2**: Extract Terraform.
After downloading, extract the Terraform package. The extraction location depends on you. Here, we'll extract it to the directory C:\Program Files\Terraform.

**Step 3**: Add Terraform to the PATH.
To use **Terraform** from any directory, you need to add it to the system's PATH.
1. In the Windows search bar, type "Advanced system settings".
2. Navigate to the **Advanced** tab and select **Environment Variables**.
![PATH](/images/2.1-terraform-install/00003.png?featherlight=false&width=26pc)
3. Select **Path** and click **Edit**.
![PATH](/images/2.1-terraform-install/00004.png?featherlight=false&width=26pc)
4. Select **New** and enter the path to the Terraform directory, then click **OK**.
![PATH](/images/2.1-terraform-install/00005.png?featherlight=false&width=26pc)
5. Check if Terraform is successfully installed by entering the command `terraform --version` in the command prompt (cmd). If the Terraform version is displayed upon entering the command, it means you have successfully installed Terraform.
![Advancedsystem](/images/2.1-terraform-install/00006.png?featherlight=false&width=50pc)
