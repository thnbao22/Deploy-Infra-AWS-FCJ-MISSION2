# DEPLOY-INFRA-AWS-FCJ-MISSION2

Tech Stack used in this project: Elastic Load Balancing, Amazon EC2, Auto Scaling Group, Amazon SNS, and Amazon Virtual Private Cloud

### Architecture

![ConnectPrivate](images/ws2-AddOns.drawio.png)

### Overview
In this lab, we will learn how to deploy a **highly available infrastructure** on AWS using **Terraform**, a popular infrastructure as code tool.

### Requirements

To do this lab, you will need to install [**Visual Studio Code**](https://code.visualstudio.com/), [**AWS CLI**](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) and [**Terraform**](https://developer.hashicorp.com/terraform/install) on your local machine.

#### AWS Account

You should have an AWS account, which has an **IAM user** with **Administrative** permission.

#### Set up Visual Studio Code
After installing **Visual Studio Code** successfully, you can download an extension for Terraform called **HashiCorp Terraform**.

![ConnectPrivate](/images/extensionTF.png)


#### Set up Terraform
You can check if the **Terraform** is installed on your local machine by opening terminal and typing `terraform version`

![ConnectPrivate](/images/CheckTF.png)
#### Set up AWS CLI version 2
You can check if the **AWS CLI** is installed on your local machine by opening terminal and typing `aws --version`.

![ConnectPrivate](/images/awsCLI.png)

#### Access keys
Next, You will need to create an **Access keys**. Following these step below to create an **Access keys**.

1. Click on your AWS account and it will appears a tab. Choose **Security credentials**.

![alt text](images/SetUp1.png)

2. Scroll down, you will see an **Access keys** interface. Click on **Create access key**.

![alt text](images/SetUp2.png)

3. In the **Create access key** interface, choose **Third party service**.

![alt text](images/SetUp3.png)

4. Then, check the square box. Choose **Next**.

![alt text](images/SetUp4.png)

5. Click on **Create access key** 

![alt text](images/SetUp5.png)

6. Click on **Download .csv file** and **Done**.

![alt text](images/SetUp6.png)

7. Open the .csv file. You will see it has an **access key** and a **secret key**.

8. Open the terminal and type `aws configure`. You will see some things appear in the terminal.

![alt text](images/SetUp7.png)

9. Configure like below:
- AWS Access Key ID: Assign **your access key**
- AWS Secret Access Key : Assign **your secret access key**
- Default region name: Enter `ap-southeast-1`
- Default output format: Enter `json`