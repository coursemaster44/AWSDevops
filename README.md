# AWSDevops
Section 2 : Getting Started
---
**2.7 Setting up your AWS Free Tier Account**

**Step-1: Open your browser and search for “Setting up your AWS free Tier Account.”**


**Step-2: Click on AWS Free Tier**



**Step-3: Click on Create Free account**


**Step-4: Provide**
- Email address,
- Password,
- Confirm Password,
- AWS Account  Name 
and click on continue.


**Step-5: Provide Contact information,address and other details.**
          
          
**Step-6: Provide Payment information and submit**


**Step-7: Authenticate yourself with OTP and Click Continue**


**Step-8: Select Free Basic Plan**


**Step-9: Select your Role and interest area.**


**Step10: Sign-In**
Provide your Email Address which was given at the creation of the account.
Click Next

**Step 11 :Provide password and Click on Sign in**

**Step 12: Click on services**

**Step13-Check  All services**

**Step14: Goto https://aws.amazon.com/free**
Note-:-This free tier account is valid for 12 months

**Step15- Scroll down to see the limit for Amazon Ec2 is 750 hrs.**

**Step16- Creating billing alert**
- Go to AWS Console>Your profile>My Billing dashboard


**Step17:This Billing alert is only created as Global.**

- Click on Billing Preferences under Preferences tab

**Step 18:Select Receive Free tier Usage Alerts and Provide your Email address**
- Select Receive Billing alerts> Click to Save preferences

**Step-19: For receiving alert One should Create alert in Cloudwatch(Monitoring service)**
         - Open CloudWatch by going AWS Console>All services>CloudWatch>Billing

**Step-20: Please Switch Region**

**Step-21:Change the Region to US East (N.Virginia)**

**Step-22: Click on CloudWatch>Billing>Create Alarm**

**Step-23: Scroll Down to conditions and define Threshold value to-5 USD**
           - Click :Next


**Step-24:** 
(a)Configure actions
(b)Notification-In-alarm
(c)Select an SNS Topic-Create new topic
- Provide-Topic Name
- Provide-Your Email to receive notification
- Click-Create topic

**Step-25:Open your mailbox and Validate the Topic subscription by Clicking on Confirm subscription.**


**Step-26: Clicking on Confirm Subscription will show you the following message.**

**Step-27: Goto :AWS Console>All services>SNS**
- See that Topic has confirmed subscription.

**Step-28: Goto Step21 and Click on Next**

**Step-29: Give Alarm name to Billing Alarm1**
- Click Next

**Step-30:  Review and Click Create Alarm**

**Step-31. See that alarm has been created Successfully.**






2.8  IAM User Set-up
---

**Step-1:Goto AWS Console>All Services>IAM>Users**

**Step-2: Click Add user**

**Step-3: Type user name- DemoUser**
- A.Select Programmatic access 
- B. Select AWS Management Console access
- C.Console password-provide Custom Password 

- **Click on Permissions**


**Step-4:  Click on- Attach existing policies directly** 
- Select- AdministratorAccess in Policy name
- Click Next:Tags


**Step-5: Click Next :Review
and Now Click on Create User**


**Step-6: Click to Download.csv
You will not have access to the secret keys again after this step.**


**Step-7: Verify Download.csv file for User name and Password.**

**Step8 : IAM Dashboard>Users>Demouser**
            - Verify the created Demouser 
            - Click on Demouser and see the access of the Demouser.**

**Step-9:Click on Permissions**

**Step-10:  Now Go to Your PC and open the Command prompt  and type-”aws configure” 
Provide your Access key Id and Secret Access key which was downloaded in Step6.**

**Step11- To Login via console paste the download link in the browser.**
- IAM user name-Demouser
- Give Password and click on Sign In
- https://course-master1.signin.aws.amazon.com/console


**Step12- See the console of  “Demouser”**

2.9 AWS CLI set-up on Windows
---
**Step-1: Go to https://aws.amazon.com/cli/**

**Step-2: -Click on 64-bit in the Windows section and download it.**

**Step-3:- Open the downloaded file(AWSCLIV2.msi) >Right click > Install **

**Step-4:- Click on Next**

**Step-5:-  Accept the license agreement and click Next**

**Step-6:- Click on Browse..**

**Step-7:- Select the destination Folder name**

**Step-8:-  Click on Next**

**Step-9:- Click on Install**

**Step-10:- Click on Finish**

**Step-11:- Open Local PC and Go-to Start>Command prompt>Run-as-administrator**

**Step-12:- Type aws --version to see the version of AWS CLI**

**Step-13:- Type “aws configure”**
- Give the value of Aws secret access key and Access key id 

**Step14- Type “aws s3 ls” command to see the list of buckets in S3.**






2.11 Download & install Git on Windows
---

**Step-1: Open internet Browser and Search for Download git for windows. 
Click on "Downloads git" link**

**Step-2:- Click on Download 2.28.0 for windows**

**Step-3:-  Click on the downloaded file GIT-2.28.0-64-bit.exe**

**Step-4:-- Click on Run**

**Step-5:--Click Next **

**Step-6:- Select Destination Location and Click on Next**

**Step-7:- Select Components and  Click on Next**

**Step-8:-  To continue,click Next.If you would like to select a different folder,click Browse.**

**Step-9:- Select Use Git from the Windows Command Prompt**
- Click on Next

**Step-10:-Select Use the OpenSSL library and Click on Next**

**Step-11:-- Select Checkout Windows-style,commit unix style and Click on Next**

**Step-12:- Select Use MinTTY and Click Next**

**Step-13:- Select Enable file system caching and Enable Git credentials Manager and Click Next**

**Step-14:-- Click Install**

**Step-15:--- Installation has been started**

**Step-16:- Select Launch Git bash**
- Click on Finish

**Step-17:- Open Local PC and Goto Start>Git Bash**

```
Type #“git init” to initialize the git
Type  #“mkdir” to make a new directory(folder)
Type # “cd test” to move into test directory

```

**Step18- Goto the path (c>users>owner>.git) -C:/Users/Pranav/.git/  as in the above to see the “test” folder just created**
```
Step 19 - Type #“git help config”
```

in Git Bash to see the manual page for git(it will open in browser when you type the command)** 
```
Step 20 -Type # “git init” to initialize 
```
- After running git init, adding and committing files/directories is possible.

``` sh
Step21-  Type # “git status”
```


git status will return the current working branch. If a file is in the staging area, but not committed, it shows with git status. 

**Step22 -  Create one file manually in test folder and see what happens--
Now type git status again in git Bash--**
```
Step23 -Type # “ git add .”
```
This command adds one or more to the staging area.
Then type git status to see the status.
```
Step24-  Type #git commit -m”first commit”|
```
This command records or snapshots the file permanently in the version history.
```
Step25-  Type # git status 
```
```
Step26-  #git log 
```
This command is used to list the version history for the current branch.


















Section 3 : AWS Basics
---

2.IAM Introduction
---
**Step1- Open AWS Console>Services>IAM>Roles**

**Step2- Click on Roles**

**Step3- Click on create Role**

**Step4- Select AWS Service as EC2**
  - Click on Permissions

**Step5- Search for S3 and Select Amazons3FullAccess and click on Next Tags**

**Step6- Click Next:Review**

**Step7-Give name of Role as “S3readOnlyAccess-demo and Click on create role**

**Step8- Type demo in Search Bar and verify the Role Created**
 - Click on “S3readOnlyAccess-demo”

**Step9- Click on Permissions>AmazonS3FullAccess**

**Step10-Please Note that in JSON Policy there are three things to see-**
- Resource,
- Action,
- Effect

**Step11- Click on Roles>S3readOnlyAccess-demo>Trust Relationships >Edit Trust relationship**

**Step12-  In Edit Trust relationship-Please Note that in JSON Policy there are four things to see-**
- Effect
- Principal
- Service
- Action



3.IAM Hands On
---
### Creating IAM User(Console)

**Step 1.Goto AWS Console>All Services>IAM>Users**

**Step 2. Click Add user**

**Step3 . Type user name- DemoUser**

- A.Select Programmatic access 
- B. Select AWS Management Console access
- C.Console password-provide Custom Password 

- Click on Permissions

**Step4:  Click on- Attach existing policies directly** 
- Select- AdministratorAccess in Policy name
- Click Next:Tags
- Click Next :Review

**Step5:     Click on Create User**

**Step 6: Click to Download.csv**
- You will not have access to the secret keys again after this step.

**Step7- Verify Download.csv file for User name and Password.**

**Step8 : IAM Dashboard>Users>Demouser**
            - Verify the created Demouser 
            - Click on Demouser and see the access of the Demouser.

**Step9-Click on Permissions**

**Step 10:  Now Go to Your PC and open the Command prompt  and type-”aws configure”**
- Provide your Access key Id and Secret Access key which was downloaded in Step6.

**Step11- To Login via console paste the download link in the browser.** 
- IAM user name-Demouser
- Give Password and click on Sign In
- https://course-master1.signin.aws.amazon.com/console

**Step12- See the AWS Management Console of  “Demouser”** 



5.EC2 Hands On
---
### EC2 Introduction
**Step1-AWS Console>All Services>Compute>EC2**

**Step2- Click on Launch instance**

**Step3- Select AMI as Amazon Linux2**

**Step4- Select Instance Type General purpose t2.micro**
 - Click Next:Configure Instance Details

**Step5-  Keep settings default for as of now**
       - Click Next :Add storage

**Step6- Add Storage-Do nothing**
           - Click Next:Add Tags

**Step7- Add tags :Type Name in key and demo in value.**
           - Click on Next:Configure Security Group.

**Step8- Create a new security group and click on add rule**
- Add rule for HTTP,Port 80 and SSH ,Port 22 
- Provide security group name as “Demo-SG”
- Click on Review and Launch

**Step9--Click on  launch**

**Step10-- Select Create a new key pair**

**Step11- Give key pair name as Demouser**

**Step12-  Download the key pair and Click on Launch Instances.**

**Step13- Launch Status-Your Instance is now Launching.**
- Click on Instance id i-0c1625ec53699abdb

**Step14- Your Instance would take approx 1 min from Instance state Pending to Running.**
- After the Status check 2/2 are initialized Instance is ready for use. 

**Step15-  Select the instance Demo and click on Connect**

**Step16- There are 3 options to connect with this instance. We will choose an “EC2 instance connect”.**

**Step17- Click on connect**

**Step18- Now you are connected to EC2**




### 7. VPC Hands ON

### Default VPC:-

**Step1-  Goto AWS Console>All Services>VPC>VPC Dashboard.**

**Step2- Click on VPCs-**

**Step3- See Default subnets-Goto VPcs Dashboard>Subnets**

**Step4-   Goto VPcs Dashboard>Route Tables**

- 4.1 There are two entries : a. to allow instances within the VPC to talk to each other. b. To allow instances inside the subnet(s) associated with this RT to be able to connect to the internet.
- 4.2 The two subnets are implicitly associated with this RT.

**Step5- VPC Dashboard>Internet Gateway**
- This IG is attached with the default VPC.

**Step6- VPC Dashboard>Security>Security Groups**
- 6.1 All instances associated with this SG can ping/talk to each other.
- 6.2 All traffic is allowed out from this SG.

**Step7- VPC Dashboard>Security>Network Acls**
- 7.1 Everything (All the traffic) is allowed into this NACL.
- 7.2- Everything (All the traffic) is allowed out of this NACL.

### Custom VPC

**Step1- Goto AWS Console>All Services>VPC>Your VPCs>Create VPC**
- Click on “Create VPC” button in the Top right corner.

**Step2- Create VPC**
- 2.1  Give Name as “Custom-vpc” and give IPv4 CIDR block as “10.0.0.0/16”
- 2.2 Scroll down and Click on Create VPC
- 2.3 vpc created successfully.Check the details.
- 2.4   This Custom-vpc has created the following things with this VPC.
       1-Route Table
       1-Security Group
       1-Network ACL
- 2.4(a) VPC>Route Tables.See the Custom-vpc Route Table
- 2.4(b) VPC>Security groups .See Custom-vpc Security group

All instances associated with this SG can ping/talk to each other.
All traffic is allowed out of this SG.

- 2.4(c) Custom-vpc NACL
All traffic is allowed into this NACL.
All traffic is allowed out of this NACL.

**Step3- Create Subnet**
- 3.1  AWS Console>All Services>VPC>Subnets>Create Subnet
- 3.2- Give Name as “Public-Subnet” 
       IPv4 CIDR block as “10.0.1.0/24”
       Click on Create.
- 3.3 AWS Console>All Services>VPC>Subnets>Create Subnet
      Give Name as “Private-Subnet” 
       IPv4 CIDR block as “10.0.2.0/24”
       Click on Create.

**Step4-Create Internet Gateway**
- 4.1  Goto AWS Console>All Services>VPC>Internet Gateways-
       Click on “Create Internet gateway”
- 4.2 Type  name as “Custom-IG”
      Click on Create Internet gateway.
- 4.3 Internet gateway is created but state is showing “Detached”
- 4.4 For attaching it with Custom-vpc select Custom-IG and Click on Actions>Attach to VPC
- 4.5  Select Custom-vpc and click on Attach Internet gateway.
- 4.6 Internet gateway is attached with Custom-vpc successfully.

**Step5-Create Route Table**
```
5.1 Goto AWS Console>All Services>VPC>Route Tables
       Route Table ID “rtb-07838fd89b3f87e18” is default Route Table Created with “Custom-vpc”
5.2 Click on Routes>Edit Routes 
     It is showing Destination as Locally.
5.3 Click on Add route 
      Put Value of Destination as “0.0.0.0”and Target as “Custom-IG”
     Click on Save routes.
5.4  See the Destination is added as “0.0.0.0” for going to the internet via internet-gateway.
5.5  AWS Console>All Services>VPC>Route Tables>Create route table
5.6 Type Name-tag as “Custom-RT” and select “Custom-vpc”
        Click on Create.
5.7  Custom-RT route table has been created.
5.8  AWS Console>All Services>VPC>Subnets
      Click on Public-Subnet and check the Destination settings.
      Public-Subnet is associated with Default-RT
5.9 Now Click on Private-Subnet see the Destination Settings.
     Click on Edit route table association.
5.10  See the route table association
5.11 Associate this Private-Subnet with Custom-RT
5.12 Now see the destination is Local
5.13 Click on Public-subnet and check the “Auto-assign public IP” settings is NO
5.14 Click on Actions>Modify auto-assign IP settings
5.15 Modify auto-assign IP settings.
5.16 Click to Check the option”Enable auto-assign public IPv4 address”
        Click on save.
5.17  Now Auto-assign public IP is showing as “Yes”
```

**Step6-Create Security Group**
```
6.1 AWS Console>All Services>VPC>Security Groups>Create security group
6.2 Give name as “Custom-SG” and select VPC as Custom-vpc
6.3  Inbound rules---- In Type select HTTP ,Port 80
       Outbound rules----All Traffic(Not a good practice).
6.4  Click on Create Security Group
6.5 Security group”Custom-SG” is created successfully.
```

**Step7-Launch EC2 with Public IP**
```
7.1  AWS Console>All Services>EC2>Launch Instance
7.2 Select AMI as Amazon Linux 2 AMI
7.3  Select instance Type General purpose,t2.micro
       Click on Configure Instance Details
7.4 Only do following changes in this step---
       Network---Custom-vpc
       Subnet---Public-Subnet
      Auto assign public Ip-Use Subnet setting(enable)
7.5 Scroll down to bottom and Put user data as following and click on Next:Add Storage
7.6 click on Next:Add Tags
7.7 Type “Name” in key and “Custom-ec2” in Value
      Click on Next:Configure security group
7.8 Select “Custom-SG” as security group.
     Click on review and launch
7.9 Please ignore the following warning as we will connect with EC2 Instance manager
Click on Continue.
7.10  Click on launch

7.11 Create a new key pair give key pair name and Click on Download key pair
       Click on Launch Instances.
7.12 Click on Instance-id
7.13 Goto EC2 dashboard and select the Custom-ec2 instance.
       See that “Public IPv4 Address” is given for this instance as we enable “Auto-assign     public Ip ”
7.14 Check the URL and see that it is live.
```

**Step8-Launch EC2 with Private IP**
```
8.1 Choose AMI-Linux2
8.2  Choose Instance type-t2.micro
8.3 Configure Instance -
Network-Custom-vpc
Private-Subnet
Auto assign Public IP-Use Subnet setting(Disable)   
8.4 Add Storage-No Change
8.5 Add tags-
Key-name
Value-Custom-ec2-private
8.6 Configure security group
8.7 EC2 instance will be created with no Public IP.
```























### 9. ELB Hands On

Elastic Load Balancing
--- 
**Step1- Go to AWS Console>All Services>EC2>Load Balancing>Load Balancers>Create load balancer**

**Step2- Select load balancer type from three given load balancers.Note We need Ec2 instances to serve the traffic.After Creating Ec2 instances in next step we will come back to this step.**

**Step3- Launch two EC2-instances for serving the Traffic of Load Balancer.**
See-Step7-Launch EC2 with Public IP

**3.1 AWS Console>All Services>EC2>Launch Instance**
```
3.2 Select AMI
3.3 Choose-Instance Type as General purpose t2.micro
3.4 Keep the things default,select the Subnet in us-east-2a AZ.
Provide following User Data and And Click on Next:Add Storage
3.5 Click Next:Add Tags
3.6 Click on Next:Configure Security Group
3.7 Create a new security group.Give name to Security group as “course-master-sg” and Select Type-HTTPand Port-80
3.8 Click Review and launch
3.9 Click on  Launch.
3.10 Select “choose an existing key pair”
       Select key pair
      Click on Launch Instances.
3.11 Click on View Instances.
3.12 Copy the IP of Instances and check in browser that they are serving the traffic -
```
**Step4- Click on Create in Application Load balancer.**

**Step5- In Basic Configuration**

- Give name-     ”course-master-elb”
- In Scheme- internet-facing
- Listeners- HTTP protocol and port-80

**Step6- Select the Availability Zones and Click on Next:configure security settings.**

**Step7- Create a security group with the name”elb-sg-group”  with port 80 open to the world for accessing from the internet.
And click on Configure Routing**

**Step8- In Target Group**
           - Select -New target group
           - Name-”ELB-TG”
           - Target type- Instance
           - Click on Next:Register Targets

**Step9-  Select the instances to add them in Registered targets**  
             - Click on Next:Review.

**Step10- Check all the settings before continuing and Click on Create.**

**Step11- Successfully created load balancer now Click on Close**

**Step12-Click on the load balancers> click on “course-master-elb” load balancer.**
- See that it is in a provisioning state.
Wait for some time.

**Step13- See now it is in active state**

**Step14-Copy the URL(DNS name) of load balancer**

**Step15- This is the URL for Application Load Balancer and Traffic is served by two EC2 behind ALB.**
- Course-master-elb-218574868.us-west-2.elb.amazonaws.com
- Copy this URL and paste it in Browser.
- This is the first EC2 instance with IP-172.31.22.19

**Step16-Refresh the Browser and see that IP has changed to IP-172.31.56.72 as traffic is served by another ec2 instance now.**
Practical has been completed now Terminate your ec2 instances and load balancer for avoiding any kind of charges by AWS.
- Select your load balancer >Actions>delete.













10.Autoscaling Introduction & Hands On
----

Auto Scaling
---

**Step1-AWS Console>All Services>EC2>Auto Scaling>Launch Configuration.**

**Step2- Give name as “Demo-lc” and select AMI(Copy it from Ec2 Launch Instance)**

**Step3- Select instance type t2.micro and click choose.**
           - In Advanced details section,you can give User data:.

**Step4- keep storage as default**

**Step5-In security group keep name as default Add rule for HTTP,Port 80.**

**Step6- select existing key pair and click on Create launch configuration.**

**Step7- launch configuration is created.**

**Step8- Click on launch configuration “Demo-lc ” >actions>create auto scaling group**

**Step9-Give auto scaling group name-**

**Step10- See launch-configuration and click on Next.**

**Step11-Select default vpc and subnets in two regions.**
- Click Next

**Step12- Keeping things Default and Click Next**

**Step13-Group size- Desired-1,Minimum-1,Maximum-1**


**Step14-Scaling policies-None ,Click Next**

**Step15 -Click next**

**Step16- Add tags**

**Step17- Review**

**Step18- Click on Create Auto Scaling Group.**

**Step19- Auto Scaling group”demo-asg” created successfully.**


**Step20-  AWS Console>All Services>EC2 Dashboard**
“1”Instance is running

**Step21- Now goto   AWS Console>All Services>EC2>Auto Scaling Group>demo-asg>Edit**

**Step22-  Editing Group Size as Desired-3,Minimum-3,Maximum-3**
            - Click on Update.

**Step23- AWS Console>All Services>EC2 Dashboard**
          - See that 2 instances are adding to get the desired 3.

**Step24- Check that all the 3 Instances are Up and Running.**




































### 11. S3 Introduction & Hands On


**Step1- Open AWS Console>All Services>Storage>S3**

**Step2-  Click on Create Bucket**

**Step3- Give Name as “myawsbucket-02112020”**

**Step4-Bucket settings for Block public Access**
- If you want this bucket as Public Uncheck “Block all public access”

**Step5-  Versioning step**

**Step6-Click on Create Bucket.**

**Step7- Bucket is created successfully.**

**Step8-Click on theBucket**
- Click on Upload

**Step9 -Click on Add files and select the file to upload.**

**Step10-  scroll down do Changes in ACL to give public access.**

**Step11-  Select file and Click on Upload**

**Step12- Select Storage Class as Standard.**

**Step13-Server-side encryption settings-Disable**
- Access control list (ACL)-Select Everyone(Public access)
- Keep rest of the things default and click on Upload,

**Step14-  See Upload status-Succeed.Click on the file uploaded.**

**Step15- Access denied error in the Browser because this file is not Public.**

**Step16-Open file and click on Make public.**

**Step17- Now Open it the Browser**
            -It is accessible.
            
**Step18- Bucket Policy**
- See your Bucket it is showing as “Objects can be Public”

**Step19-  For making it Full Public we need to edit Bucket Policy**

- Amazon S3>myawsbucket-02112020>permissions>Bucket policy
- Copy the following policy in that section- and click on save.
```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicRead",
            "Effect": "Allow",
            "Principal": "*",
            "Action": [
                "s3:GetObject",
                "s3:GetObjectVersion"
            ],
            "Resource": "arn:aws:s3:::myawsbucket-02112020/*"
        }
    ]
}
```
**Step20- Bucket is now Public.**

**Step21-Versioning**
-Check if the versioning is enabled or not.

**Step22-- To see the versioning function.Create the following Demo file and save it in your local PC.**

**Step23-  Open bucket and click on Upload And make the file public.**

**Step24- Check the output of file.**

**Step25-Edit the file and upload it again and make it Public.**

**Step26-  This version is  the latest version.To see all version click on List versions**

**Step27- Open the latest version and see the difference.**










































### 12. Cloudwatch Introduction & Hands On

**Step1- Goto AWS Console>All Services>CloudWatch>Events>Get started**



**Step2- You will see the Following Screen.**


**Step3- In Event Source---**
      - Select Event Pattern and then 
      - Click on Build event pattern to match as “events by service” 
  
**Step4 -In Service Name-Select” Ec2 “**
                 - Event Type-”Ec2 Instance State-change Notification”
                 - Select Specific state as “stopping”
                 - Select Any Instance
                 - Click on Add target in Targets Tab
   




**Step5- Select SNS Topic as “Ec2Stopping-CWevents” in Targets**
             ****To create SNS Topic See next Step6

**Step6- Create SNS Topic**
 - 6.1  Goto AWS Console>All service>Simple Notification Service>Create Topic
         Give name as Ec2Stopping-CWevents 
- 6.2 Click on Create Topic
- 6.3 Topic Created Successfully.Now Click on Create subscription.
        
- 6.4  Select Protocol as Email and endpoint as “coursemaster44@gmail.com”.Now Click on Create subscription.

- 6.5 Subscription created successfully.
      - Status is showing Pending confirmation.
      - To confirm this subscription check for the message from<no-reply@sns.amazonaws.com>    in your Email Inbox.
      
- 6.6 Check the Email Inbox or Spam
       - In my case it arrived in Spam
       - Click on “Confirm subscription”

- 6.7 Subscription Confirmed.

- 6.8 Now goto Amazon SNS >Topics>Ec2Stopping-CWevents
     - Status is confirmed.

**Step7- Goto Step5**
          - Click on Configure details.

**Step8- Configure Rule-**
            - Give name as “ec2stoppingRule” and Description “ec2stoppingRule”
            - Keep state enabled
            - Click on Create rule

**Step9 - Rule created.** 
      
**Step10 -Goto AWS Console>All Services>EC2>EC2 Dashboard.**
           - In my Case one Instance is Running.
                      
- Click on Instance>Actions>Instance State>Stop Instance

- Click on Stop



**Step11-  Instance is in stopping stage**


**Step12- Check your Email from <no-reply@sns.amazonaws.com> which was given in Subscription of Topic.**


You can detect and react to changes in the state.




CloudWatch Alarm
---

**Step1 -Goto AWS Console>All Services>CloudWatch**
 
**Step2- Click on Alarms>Create Alarm**

**Step3 -Click on Select metric**

**Step4- Select Ec2 in All metrics**

**Step5- Click on per-Instance metrics**

**Step6 -Goto AWS Console>All Services>Ec2 dashboard and copy Instance-id**
             
**Step7 - Now Paste it in the search bar-**

**Step8 -Click to Select CPUUtilization**

**Step9 -Click on select metric**

**Step10- No action in Specify metric and conditions.**
             
**Step11 -Scroll down and come to Conditions.**
- Threshold type-static
- Whenever CPUutilization is -Lower
- Than define the threshold value-40


**Step12 -In Notification**
        - Alarm stage trigger-In Alarm
        - Select an SNS topic(See-Create SNS Topic) -select an existing topic
        - Send a notification to--Ec2Stopping-CWevents
        

**Step12-Scroll down and come to Ec2 action.**
     - Alarm stage trigger--In Alarm
     - Take the following action--select stop this instance
     - Click on Next



**Step13- Give Alarm name-My-alarm**
            - Click on Next
              

**Step14- Preview all the details and click on “create alarm”**

**Step15- Alarm created successfully.**
          - See in Alarms My-alarm is showing “Insufficient data”
           - Hit refresh button

**Step16- State is showing In-alarm**

**Step17- Check you Email and you would see the following email.**

**Step18- Check the instance in EC2-Dashboard.**
         - It is showing stopped as per Cloudwatch Alarm configuration.






























### 14. DynamoDB Hands On


Dynamo DB
---

 **Step1- AWS Console>All services>DynamoDB**
 **Step2- Click on Create table**
 **Step3- Give Table name-Course master**
          - Primary key-id
 **Step4- Check  that the storage is 0 bytes**
 **Step5- click on items>create item**
 **Step6- click on + button**
 **Step7-  - enter id -101
       	 - Name-ram
           - Mobile-0123123123  and click on save.
 
**Step8- check the entry in Items**

 **Step9- create another  item with following details.**
- Id-102
- Address-delhi
- mobile-0120120120120

 **Step10 check the entry**
 
**Step11-third entry was also done with the same process.**
 
**Step12- See there are 3 entries.**
 
**Step13- now select scan and click on add filter put the value -mobile,number,exists**
 	You will get therow for entry with mobile
 
 **Step14- AWS Console>dynamoDB>Create table**
 Now click on Query in partition key select id and in number-102
 See the with details.
 
 **Step15-now create a table with a primary and sort key.**
           - Partition key-name
           - Sort key- last name
 **Step16-put the value for name-shankar,last name-singh**
        - Click on save
 **Step17-See your table details.**
 
**Step18- Actions>Duplicate**

 **Step19-Put the value for entry name-ramesh for which you want to duplicate.**
 
 **Step 20 Click on save**
 
 **Step21 check for the duplicate entry just created.**
 
 **Step22- To delete items Actions>Delete>select item >delete**
 
 **Step23-Item is deleted.**
 
 **Step24- For Deleting table select table and click on delete table.**
- Type delete click on delete





16.Elastic Beanstalk Hands On
---

**Step1- Create an application and an environment**
- Goto-https://console.aws.amazon.com/elasticbeanstalk/home#/gettingStarted?applicationName=getting-started-app

- Name-getting-started-app

**Step2- Platform-Node.js**

**Step3- Platform version--recommended**
           - In Application code-select Sample Application
           - Click on Create Application


**Step4- Creating environment started-**
Elastic BeanStalk launches an environment named GettingStartedApp-env with these AWS resources:
```
1.S3 Bucket
2.Target Group
3.Security Group for ec2 instance
4.Security Group for ALB
5.Auto Scaling launch configuration
6.Auto Scaling Group
7.Auto Scaling Policies
8.CloudWatch Alarms
9.Load Balancer
10.Load balancer listener
11.EC2 instance
``` 
 
 **Step5 -Check the environment.**

**The environment overview pane shows  its name, its URL, its current health status, the name of the currently deployed application version, and the platform version that the application is running on.** 
Below the overview pane you can see the five most recent environment events.

 - Click on Go to environment

**Step6- Goto each component and verify the resources created by Elastic BeanStalk--**

**6.1 S3 Bucket**
  - Goto AWS Console>All Services>S3>Buckets

**6.2  Target Group**
 - Goto AWS Console>All Services>EC2>Load Balancer>Target Group**

**6.3-Security Groups**
- Goto AWS Console>All Services>EC2>Security Groups**

**6.4  Auto Scaling launch configuration-**  
- AWS Console>Services>Ec2>Auto Scaling>launch configuration**



**6.5  Auto Scaling Group**
- AWS Console>Services>Ec2>Auto Scaling>Auto Scaling Groups

**6.6   Auto Scaling Policies-Scale Down,Scale Up**
- AWS Console>Services>Ec2>Auto Scaling>Auto Scaling Groups>Click on AS group Created>Automatic Scaling

**6.7  CloudWatch Alarms-**
- AWS Console>Services>CloudWatch>Alarms>Alarm

**6.8  Load Balancer**
- AWS Console>Services>EC2>Load Balancing>Load balancers

**6.9   Load balancer listener**
- AWS Console>Services>EC2>Load Balancing>Load balancers>select load balancer>listeners

**6.10  EC2 instance**
- AWS Console>All services>EC2 >Instances>      
- See the instance.All Checks has been completed.
- Check Elastic BeanStalk AWS resources List.


**Step7- Terminate the environment.**
- AWS Console>All Services>Elastic BeanStalk>Getting-started-env>Actions>terminate environment



Section 5 : Git, Github, and CodeCommit
---

**2. Installing Git & Creating a local git repository**

### Installing Git

**Step1- Open internet Browser and Search for Download git for windows.** 
Click on Downloads git link

**Step2- Click on Download 2.28.0 for windows**

**Step3-  Click on the downloaded file GIT-2.28.0-64-bit.exe**

**Step4-- Click on Run**

**Step5--Click Next**

**Step6- Select Destination Location and Click on Next**

**Step7- Select Components and  Click on Next**

**Step8-  To continue,click Next.If you would like to select a different folder,click Browse.**

**Step9- Select Use Git from the Windows Command Prompt**
- Click on Next

**Step10-Select Use the OpenSSL library and Click on Next**

**Step11-- Select Checkout Windows-style,commit unix style and Click on Next**

**Step12- Select Use MinTTY and Click Next**

**Step13- Select Enable file system caching and Enable Git credentials Manager and Click Next**

**Step14-- Click Install**

**Step15--- Installation has been started**

**Step16- Select Launch Git bash**
- Click on Finish

**Git Has been installed.**

Create a Local Git Repository
---

- 1.	In VS Code, Open Terminal : “Terminal” menu-> New Terminal

- 2.	Create a directory “git-demo” : mkdir git-demo

- 3.	Move into this directory : cd git-demo

- 4.	Initialize git in this directory : git init

- 5.	Signup + Login/Login into github

- 6.	Create a repository called “git-demo” : Repositories-> New-> Type “git-demo” in “Repository name” text-box. Check the radio button “Public”. Don’t    click/select anything else. Click on “Create repository”.

- 7.	Connect “git-demo” local repository/directory with “git-demo” remote repository on github : git remote add origin https://github.com/singhamit9/git-demo.git

- 8.	Open .git/config file in terminal : cat .git/config . You will find an entry :
[remote "origin"]
url = https://github.com/singhamit9/git-demo.git

9.	Create .gitignore file : touch .gitignore

10.	Open .gitignore and add these two entries:
node_modules/
.DS_Store . Save the file.

11.	Check status of file tracking by git and add newly added/modified files to git tracking : git status -> git add .gitignore

12.	Commit .gitignore to local repository : git commit -am “First commit”.

13.	Push first commit to remote github repository : git push -u origin master

14.	Copy the following files and folders from node-project directory : package.json, public, src, templates, deploy_scripts, appspec.yml, buildspec.yml to git-demo directory.

15.	Check status of file tracking by git and add newly added/modified files & folders to git tracking : git status -> git add .

16.	Commit these files & folders to remote github repository : git push -u origin master

17.	Refresh the github page with repository git-demo. You will see all your latest commits (changes) here.




3.Create a remote Git repository & connect with local git repository
----


- 1.	Signup + Login/Login into github

- 2.	Create a repository called “git-demo-1” : Repositories-> New-> Type “git-demo” in “Repository name” text-box. Check the radio button “Public”. Check the  checkbox “Add a README file”. Click on “Create repository”.

- 3.	Click on dropdown menu “Code” -> Ensure HTTPS tab is selected  -> Copy the HTTPS URL underneath.

- 4.	In VS Code, Open Terminal : “Terminal” menu-> New Terminal

- 5.	Ensure you are in the directory where you want to clone this remote repository. For me, it is ~/Documents/CICD : cd ~/Documents/CICD .

- 6.	Clone the remote Github directory : git clone https://github.com/singhamit9/git-demo-1.git (this is the url you copied from github in step 3)

- 7.	Move into the newly created directory/local git repository : cd git-demo-1

- 8.	Open .git/config file in terminal : cat .git/config . You will find an entry :
[remote "origin"]
url = https://github.com/singhamit9/git-demo1.git

- 9.	Create .gitignore file : touch .gitignore

- 10.	Open .gitignore and add these two entries:
node_modules/
.DS_Store . Save the file.

- 11.	Check status of file tracking by git and add newly added/modified files to git tracking : git status -> git add .gitignore

- 12.	Commit .gitignore to local repository : git commit -am “First commit”.

- 13.	Push first commit to remote github repository : git push -u origin master .

- 14.	Refresh the github page with repository git-demo-1. You will see all your latest commits (changes) here.








Introduction To AWS CodeCommit
----

- 1.	Sign in into your AWS account with the root user.

- 2.	In the “Find Services” textbox, type “IAM” and click on IAM.

- 3.	Under “Access Management”, click on “Users”-> click on “Add User”

- 4.	In the “User-name” text box, type the name of the user you want to create (in this case : “course-master”). Check “Programmatic Access”, and “AWS  Management Console access” checkboxes. Click on the “Custom Password” radio box and type the password you want. Uncheck, “Require password reset” and click on “Next: Permissions” button.


- 5.         Click on “Attach existing policies directly”-> check the checkbox for “Administratoraccess”-> click on “Next: tags” button.

- 6.	Click on “Next: Review”.

- 7.	Click on “Create User”.

- 8.	Click on “Download .csv” -> click on close

- 9.	Click on “Dashboard” -> click on “Customize” next to sign-in link.

- 10.	Type Account Alias and click on “Yes, Create”.

- 11.	 Note the modified “IAM User sign-in link”: https://course-master.signin.aws.amazon.com/console

- 12.	Sign out of AWS console.

- 13.	Sign in using this URL : https://course-master.signin.aws.amazon.com/console

- 14.	Type User-name in “IAM user name” text box, and password in “Password” text box -> click on “sign-in” button.

- 15.	In the “Find Services” textbox, type “IAM” and click on IAM.

- 16.	Under “Access Management”, click on “Users”-> click on “course-master” username.

- 17.	Click on “Security Credentials” tab

- 18.	Scroll down and click on “Generate credentials” in HTTPS git credentials for AWS Code Commit

- 19.	Click on “Generate credentials” -> Download credentials“Close” button.

-20.	Click on “Services” ->  under “All Services”, type codecommit ->click on CodeCommit

- 21.	On the CodeCommit landing page, click on “Repositories” from left menu panel -> click on “Create repository

- 22.	 In “Repository settings”, type “Repository name” as “node-sample-ap”-> click on “Create” button.

- 23.	 Scroll down -> click on “Copy” under “Step 3 : Clone the repository”.



- 24.	Open the working directory on your local system on VS Code. In this case, ~/Documents/CICDDemo

- 25.	 Click on “Terminal” menu -> “New Terminal”

- 26.	Paste the copied URL from step 23 in terminal and hit enter

- 27.	 Type the CodeCommit username you generated in step 19 in the pop up for “Username” -> hit enter

- 28.	 Type CodeCommit password you generated in step 19 in the “Password” pop-up -> hit enter.

- 29.	A local directory/git repository “node-sample-ap” got created under your working directory (here ~/Documents/CICDDemo).

- 30.	Move into the newly created local git repository : cd node-sample-ap

```sh
- 31.	Create .gitignore file : touch .gitignore
```
- 32.	Open .gitignore and add these two entries:
node_modules/
.DS_Store . Save the file.

```
- 33.	Check status of file tracking by git and add newly added/modified files to git tracking : git status -> git add .gitignore
```
```
- 34.	First commit# Commit .gitignore to local repository : git commit -am “First commit”.
```
```
- 35.	First Push#Push first commit to remote github repository : git push -u origin master
```
```
- 36.	 Check CodeCommit repository for newly pushed commit : click on “Repositories” in the left menu panel -> click on “node-sample-ap” under “Repositories”.
```
```
- 37.	 .gitignore file is now present in “node-sample-ap” repository.
```
```sh
- 38.	Copy all the contents of ~/Documents/CICD/nodejs-web-app-with-ejs/ to present working directory (~/Documents/CICDDemo) : cp -R ../../CICD/nodejs-web-app-with-ejs/ .
```

```
- 39.	Check status of file tracking by git and add newly added/modified files to git tracking : git status -> git add .
```

```
- 40.	Commit newly tracked files to local repository : git commit -am “Second commit”.
```

```
- 41.	Push second commit to remote github repository : git push -u origin master
```

- 42.	 Check CodeCommit repository for newly pushed commit : click on “Repositories” in the left menu panel -> click on “node-sample-ap” under “Repositories”.

- 43.	Pushed files in step 42 are now present in “node-sample-ap” repository.




























Section 6 : Deploying Sample App on AWS (Without CImm/CD)
---

6.3 Setting-up ec2 Instance
---

- 3.1AWS Console>All services>EC2

- 3.2 Click on Launch Instance :

- 3.3 Select AMI Linux2

- 3.4 Choose Instance type t2 micro and Click Next:Configure Instance

- 3.5 Leave everything  default beside IAM Role and User Data Section and Click Create IAM Role
  - AWS Console>IAM>Role>Create Role

- 3.6-Now come back to EC2 Instance creation page.
   - Select IAM Role as node-sample-ap-ec2-role

3.7 Refer script for user data.
```sh
#!/bin/bash
yum update -y
yum install ruby -y
yum install nmap-ncat -y
yum install wget -y
cd /home/ec2-user
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
chmod +x ./install
./install auto
service codedeploy-agent status
```

- 3.8 Click Next:Add Storage---keep Default
   - Click Next Tags in Tags give key as name and value as deploy
  
- 3.9 Configure security groups:Give All Traffic access for as of now(not recommended in production)

- 3.10 Click on review and Launch
   - Create a key pair and download it .
  - View Instances
 
- 6.4. Pushing Sample App on CodeCommit


Step1- Code Commit-
---

- 1.1 AWS Console>All services>Code Commit>repositories>create repository>Create
    Give Name-MYRepo

- 1.2 Copy URL

- 1.3 Goto Local PC and open Git with Application Code location and type
```sh
#git init
```
```sh
1.4 #git status
```
```sh
1.5 #Git add .
```
```sh
1.6 # Git commit -m “Commit1”
```
```sh
1.7 # Git clone https://git-codecommit.us-west-1.amazonaws.com/v1/repos/MyRepo 
Provide User name and password for HTTPS Code Commit.
```
```sh
1.8 #git remote add origin https://git-codecommit.us-west-1.amazonaws.com/v1/repos/MyRepo
     Provide User name and password for HTTPS Code Commit.
```

```sh
1.9 #git push origin master
```

- 1.10 AWS Console>All services>Code Commit>repositories>MyRepo


6.6.Deploying Sample App on a single ec2
---

**Step1- Launch the Instance**
- Open AWS Console>EC2>Launch Instance

**Step2- Select AMI linux2**

**Step3- Select Instance Type as t2.micro**

**Step4- Keep all values default beside IAM Role**

**Step5- Click on Create new IAM role**

**Step6- Select EC2 and click on NEXT:Permissions tab**

**Step7- Search s3 and select s3readonly role**

**Step8- Next:Review**

**Step9- Provide the name of your role**

**Step10- Click on add storage**

**Step11- Next:Tags key:Name and value is course-master**

**Click Next Configure security group**

**Step12- Click on Review and launch**

**Step13- Click on Launch**

**Step14- Select the key pair and Click on Launch Instance**
- Instance is running .

**Step15- Now Click on Connect**

**Step16- Do the following steps manually:**
```
yum update 
yum install nmap-ncat 
curl -sL https://rpm.nodesource.com/setup_lts.x | bash - 
yum install nodejs -y
yum install git -y
git clone https://git-codecommit.us-east-2.amazonaws.com/v1/repos/node-sample-ap
cd node-sample-ap
npm install
node app.js 
```
```sh
#yum update -y
```
```sh
#yum install nmap-ncat
```
```sh
# curl -sL https://rpm.nodesource.com/setup_lts.x | bash - 
```
```sh
# yum install nodejs -y
```
```sh
#yum install git -y
```
```sh
#Git Clone “Code Commit cloning path”
```
```sh
Step17- Provide Username and password for code commit HTTPS (Downloaded earlier in Code Commit Introduction To AWS CodeCommit)
```
**Step18 - #cd node-sample-ap**
```sh
#ls
Step19 - #npm install
```
**Step20- Now Check the URL of EC2 instance.**

**Step21- Open in the internet browser**



6.7 Deploying Sample App on ec2 Fleet -1(ASG Lifecycle)
---

 **Step1- Create Launch Configuration with “test-lc” name**

**Step2- Select linux2-AMI by searching its AMI number”ami-03657b56516ab7912”**
       - Select instance type t2.micro 
       - Now select your instance profile name “CodeDeployDemo-EC2-Instance-Profile”

**Step3- Click in Advanced details section and look for user data.**
- Copy following user data(remember to edit your region) and paste it in User data as text:
```
#!/bin/bash
yum update -y && \
yum install nmap-ncat -y && \
curl -sL https://rpm.nodesource.com/setup_lts.x | bash - && \
yum install nodejs -y && \
npm install -g pm2 && \
pm2 update && \
cd /home/ec2-user && \
aws s3 cp s3://new-node-asingh/devbuildsnew/node-another-new . && \
unzip node-another-new && \
npm install && \
pm2 start -f app.js && \
sleep 10 && \
INSTANCE_ID=$(curl -s http://169.254.169.254/latest/meta-data/instance-id) && \
aws autoscaling complete-lifecycle-action --lifecycle-action-result CONTINUE --instance-id $INSTANCE_ID --lifecycle-hook-name test-hook --auto-scaling-group-name test-asg --region us-east-2 || \
aws autoscaling complete-lifecycle-action --lifecycle-action-result ABANDON --instance-id $INSTANCE_ID --lifecycle-hook-name test-hook --auto-scaling-group-name test-asg --region us-east-2
```


**Step4- Click on Create Launch Configuration**
- Launch configuration has been created.

**Step5- Now select launch configuration -> click actions  ->  create auto scaling group.**

**Step6- Give name to auto scaling group as “test-asg” and select launch configuration.**
- Click Next
- Select default VPC and default subnets in multiple availability zones.

**Step7 -Click Next**

**Step8- Select Group size:**
- Desired capacity -0
- Minimum Capacity-0
- Maximum capacity-0

**Step9- Scaling policies-None**
- Click Next

**Step10- Click Next**

**Step11- Review all the details and click on Create Auto Scaling group**
- Auto scaling Group “test-asg” has been created.

**Step12- Click on auto scaling group>Instance management tab >Create lifecycle hook**

**Step13- Type lifecycle hook name as “test-hook”**
- Lifecycle transition -Instance Launch
- Heart Beat Time-30 secs 
- Default Result Continue

**Step14- Now Click on auto scaling group and edit group size to desired-1,minimum-1,maximum-1**

**Step15- Click on update**


**Step16- Monitor the Instances in EC2 Dashboard.**
- New Instance will be created.

**Step17- Goto-EC2>Auto Scaling groups>test-asg**
- Lifecycle will show Pending>Pending wait>In service

**Step18- Check the Instance URL and paste it in the Browser.**
- URL is live.



6.7 Deploying Sample App on ec2 Fleet -2
---

**Step19- Now we will edit group size as 2-2-2 in Auto Scaling Group.**
- Desired-2
- Maximum-2
- Minimum-2

**Step20- Click Update**

- After updating the group size one more new instance will be created.
- Lifecycle tab shows the Pending> Pending wait >IN-Service

**Step21- Check Ec2 dashboard**
- New instance is running in EC2 Dashboard

**Step22- Copy the Ip Address of Instance and validate the application**



6.9 Deploying Sample App on Elastic Beanstalk
---

**Step1- Goto AWS console>All services>Elastic Beanstalk**

**Step2-  click on Create Application**

**Step3-Click on Create new Environment**
- Provide application name-”sample app”

**Step4-- In Platform section select node js**
            -In Application code select Sample Application

**Step5- Click on Create Application**
  - Creating SampleApp-env started----

**Step6-  Launches an environment named GettingStartedApp-env with these AWS resources:**
```
●	An Amazon Elastic Compute Cloud (Amazon EC2) instance (virtual machine)
●	An Amazon EC2 security group
●	An Amazon Simple Storage Service (Amazon S3) bucket (by what name?)
●	Amazon CloudWatch alarms (for what?)
●	An AWS CloudFormation stack
●	A domain name
●	Launch Configuration
●	ASG
●	Target Group
●	ALB
 ```
 
**Step7-- Click on environments and click on sampleApp-env**

**Step8--- Health is ok means that application is deployed and launched successfully.**

**Step9---  Click on Go to environment**

**Step10-  Check your application’s web page**

Sample application deployed successfully.
Don’t forget to delete your environment to avoid the charges.





Section 7 : Deploying Sample App on AWS (With CI/CD)
---

7.2 Setting up ec2 Instance 
---
**See- 6.3 Setting-up ec2 Instance**

7.4 Creating CodeBuild Project
---

**Step1.Open the AWS CodeBuild console at https://console.aws.amazon.com/codesuite/codebuild/home**

**Step2. Click on “Create Build Project” and Fill the following sections-**
 - (a)Project Configuration--Type Project Name as “node-sample-app”
 - (b)Source>Source 1-Primary Section>Select Source Provider “AWS Code Commit” from drop down menu and
 - fill the repository name “node-sample-ap” and
 - Reference Type select “Branch” and Branch as “Master”

**Step3:Environment Section--**
- Select Environment image -Managed image and
- Operating system- “Amazon Linux 2”
- Run Time as- “Standard”,
- image as -aws/codebuild/amazonlinux2-x86_64-standard:3.0 and
- image version -“always use the latest image for this runtime version”
- Environment Type- :”Linux”

**Step4-Service Role--If you do not have service role  choose “New Service Role” type      service role name - “codebuild-node-sample-app-service-role”
     If you have a service role which was created earlier then choose existing service role.**

**Step5-Buildspec section:**
Build specifications select “Use a buildspec file”

**Step6-Artifacts Section:-- To store build output artifacts choose  S3 in type,**
- Bucket name(see below for bucket creation) as “node-sample-ap-output-bucket”
- Select Zip in artifact packaging
- If you do not want your build artifacts encrypted select “Disable artifacts encryption”


**Step7- Logs section**
- Choose logs you want to create select cloudwatch logs
- Type group name as “node-sample-ap-logs”



**Step8-Building Sample App**
---

- Goto AWS Console>Developers Tools
- Click on Create build project >Start Build
- After Clicking Start Build it will show all the steps done in the previous step.

- Check build configuration Select Build type as “single build”
- Branch -master

- Review it .Choose start build

**Step 9-You can see the phase details for monitoring the ongoing build-**
```
 Check the status of every step of all phases in phase details-
SUBMITTED
QUEUED
PROVISIONING
DOWNLOAD_SOURCE
INSTALL
PRE_BUILD
BUILD
POST_BUILD
FINALIZING
COMPLETED.
```
- You can also see the build logs by clicking on build logs

- For checking output open S3 with this path s3://node-sample-ap-output-bucket/node-sample-ap


**Step10-You can check the CloudWatchlogs by selecting AWS Services>Cloudwatch>Logs>Log groups>node-sample-ap**
-Choose node-sample-ap-logs





7.8 Creating CodeDeploy Application
---
**Step1- Open the AWS CodeDeploy console at https://console.aws.amazon.com/codesuite/codedeploy/home**
- Get started with AWS CodeDeploy by creating your first deployment application
- Click on CodeDeploy>Create Application

**Step2- Enter Application name code-sample-ap-deploy in Application Configuration Section And Choose Compute platform as EC2/On-premises**

**Step3- Click on Create application**
- It will show that application created
- In the next step choose Create deployment group under deployment groups section.
- Give the name “ node-sample-ap-group” in the deployment group name section.

7.10 Deploying Sample App on a single ec2
---
**Step1- Open the AWS CodeDeploy console at https://console.aws.amazon.com/codesuite/codedeploy/home**
- Get started with AWS CodeDeploy by creating your first deployment application
- Click on CodeDeploy>Create Application

**Step2- Enter Application name code-sample-ap-deploy in Application Configuration Section And Choose Compute platform as EC2/On-premises**

**Step3- Click on Create application**
- It will show that application created
- In the next step choose Create deployment group under deployment groups section.
- Give the name “ node-sample-ap-group” in the deployment group name section.

**Step4-Provide service role in Service Role section:** 

**Step5-Now come to AWS Code Deploy>deployment group**
- Next Deployment type choose In-Place and select Amazon Ec2 instances in Environment configuration.

**Step6-In tags select key--name and value---deploy**
- Above tags values  were given during the creation of ec2 instances in tags section..
- Choose never in AWS Systems Manager section:
- In Deployment settings you can select according to your choice i am using CodeDeployDefault:Allatonce.
- In Load Balancer deselect Load Balancer for as of now.(will do it later in next session)

**Step7-Setting-up Ec2-Instance with Code deploy agent and IAM role attached for S3**
- AWS Console>All services>EC2

Refer below script for user data.
```
User Data Script :-
#!/bin/bash
sudo yum update -y
sudo yum install nmap-ncat -y
sudo yum install git -y
# add nodejs to yum
sudo curl -sL https://rpm.nodesource.com/setup_lts.x | bash -
sudo yum install nodejs -y #default-jre ImageMagick
sudo wget https://aws-codedeploy-us-east-2.s3.us-east-2.amazonaws.com/latest/install
sudo chmod +x ./install
sudo ./install auto
sudo service codedeploy-agent start
# install pm2 module globaly
sudo npm install -g pm2
sudo pm2 update
```

**Step9-Now Come back to Deployment Group**
- Provide Name,service role
- Deployment type-In-place,Env-config---Ec2 instances
- Aws systems manager --never
- Deployment settings-CodeDeployAllatOnce
- Click on Create deployment group.

**Step10-Deployment Group created now click on Create deployment.**
- See the deployment settings.

- Deployment group node-sample-ap-group is taken automatically

- Select revision type:My Application is stored in S3

- Give revision location from your s3 Build artifacts output bucket

- AWS Console>S3>Buckets>node-sample-ap-output-bucket

- Click on bucket open revision location >click on artifacts>copy path

- Paste this path to revision location option and select .ZIP from dropdown in next row.

**Step11-Click on Create Deployment**
- Deployment created successfully.

**Step12-View events in Deployment Lifecycle Events Section.**
```
APPLICATION STOP
DOWNLOAD BUNDLE
BEFORE INSTALL
INSTALL
AFTER INSTALL
APPLICATION START
VALIDATE SERVICE
```
- Deployment is completed.

- Check Ec2 Instance URL and test the Application. 

- Copy the IP Address of the Ec2-Instance and paste in the browser and Hit Enter.

- Sample app is running.Application is deployed successfully.






7.11 Deploying Sample App on ec2 Fleet -1
-----

**Step1- Creating IAM “CodeDeployDemo-EC2-Instance-Profile” Instance profile with S3 access.**

**Step2-Create Application**
- AWS Console>All services>CodeDeploy>Applications
- Fill application name as node-sample-ap-deploy and select compute platform as EC2-On premises.

Application created.


**Step3-Create Launch Configuration**
- Goto AWS Console>EC2>Launch Configuration
- Copy AMI name value from Launch instance section of EC2.

**Step4- Give Name,AMI,Instance type**
- Enter  IAM Instance profile which was created in the first step.

**Provide user data in Additional Configuration section**

- Application User data
```
#!/bin/bash
yum update -y
yum install ruby -y
yum install nmap-ncat -y
yum install wget -y
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
export NVM_DIR="/.nvm"
[ -s "/.nvm/nvm.sh" ] && \. "/.nvm/nvm.sh"
nvm install node
nvm use node
node -v
npm install npm@latest -g
npm -v
cd /home/ec2-user
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
chmod +x ./install
./install auto
service codedeploy-agent status
```

**Step5-Security Groups section:Create security group with name AutoScaling-security-group-elb and give All Traffic in Rule type source anywhere (only as of now not recommended for production)**

- Choose key pair and click on create launch configuration
- Launch configuration created.

**Step6- Select launch configuration and click the actions tab and click on create auto scaling group.**

**Step7 -Select VPC and subnets**

**Step8- Configure advanced options-keep things default** 

**Step9 -Configure Group size and scaling Policies.**
- Desired-1,Min-1,Max-1
- Scaling Policies-None

**Step10 -Add notification-No change required**
- Click next 
- Add tags Click next
- Click Review and ASG will be created.

**Step11- Goto DeveloperTools>CodeDeploy>Applications>Dynamo-db>Create deployGp**

**Step12- Deployment type-In-place**
- ENV config>amazon EC2 Auto scaling groups>SingleEc2ASG
- Matching Instances-1
- Deployment settings-CodeDeployDefault:AllatOnce
- Deselect load balancer
- Click on Create deployment group.

**Step13- Deployment group created successfully.click on Create deployment.**

**Step14- select revision location and revision type as zip**
- Click on create deployment.

**Step15- Deployment Created.**

**Step16 -Copy the Ip of Ec2 instances SeeApplication is live**







7.12 Deploying Sample App on ec2 Fleet -2
----


**Step1- Creating IAM “CodeDeployDemo-EC2-Instance-Profile” Instance profile with S3 access.**

**Step2-Create Application**
- AWS Console>All services>CodeDeploy>Applications
- Fill application name as node-sample-ap-deploy and select compute platform as EC2-On premises.

Application created.


**Step3-Create Launch Configuration**

- Goto AWS Console>EC2>Launch Configuration
       
- Copy AMI name value from Launch instance section of EC2.

**Step4- Give Name,AMI,Instance type**
- Enter  IAM Instance profile which was created in the first step.
- Provide user data in Additional Configuration section
- Application User data
```
#!/bin/bash
yum update -y
yum install ruby -y
yum install nmap-ncat -y
yum install wget -y
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
export NVM_DIR="/.nvm"
[ -s "/.nvm/nvm.sh" ] && \. "/.nvm/nvm.sh"
nvm install node
nvm use node
node -v
npm install npm@latest -g
npm -v
cd /home/ec2-user
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
chmod +x ./install
./install auto
service codedeploy-agent status
```

**Step5-Security Groups section:Create security group with name AutoScaling-security-group-elb and give All Traffic in Rule type source anywhere (only as of now not recommended for production)**
- Choose key pair and click on create launch configuration

- Launch configuration created.

**Step6- Select launch configuration and click the actions tab and click on create auto scaling group.**

**Step7- Give name node-sample-ap-elb-ASG and select launch configuration node-sample-ap-elb**

**Step8 -Configure settings for Network Select default VPC and default subnets**

**Step9- select load balancing under this select application load balancer choose target group or create new target group as per following steps.**

- Click on create target group

**Step10- In next step select instances**
- Give name TG1

**Step11- Protocol HTTP and port no. 3000** 
- Keep vpc as default.
- Keep all other settings unchanged and click on Next.
- Registration target step don't register any target as of now click on create target group.
- Target Group Created .
- Now come back to Creating auto scaling group

**Step12- In the next step keep desired capacity,minimum capacity,maximum capacity zero.
Change it later.**

**Step13- Scaling policies- None**
- Click next

**Step14- Click Next**

**Step15- Click next**

**Step16- Review your given information **

**Step17- Click Create auto scaling group.**
- AWS Console>EC2>Auto scaling groups
- You can see the newly created auto scaling group.Next task is to create Load balancer

### Create Load balancer

**Step18- AWS Console>EC2>Load balancers>create load balancer**

**Step19- Give name node-sample-ap-elb**
- Scheme-internet facing
- Ip address type-ip4
- In Listeners protocol is HTTP and Port is 3000.
- Vpc-default,select availability zones.

**Step20- Click configure security group**

**Step21- All traffic access for as of now.**
- Next configure routing
- Next register targets-do not register any targets
- Review>>create load balancer
- Wait for the load balancer to come provisioning to the active stage.

_ Now all the necessary steps are done.We can move further for the new deployment with an auto scaling group.
- First of all edit the Auto Scaling Group settings to 2 for desired,2-min and 2-max

**Step22- Update**
- This will add 2 new instances check in ec2 dashboard

## Create Deployment group

**Step23- Now goto AWS Console>All Services>CodeDeploy>applications**
- Click on application node-sample-ap
- Click on create deployment group

**Step24- Deployment type in-place**
- Environment configuration select Amazon EC2 auto Scaling groups and select the node-sample-ap-elb-asg from dropdown
- Select deployment settings as per your choice
- In the load balancer tab select the enable load balancing and select application load balancer under it.
- Choose target group TG1 
- Click on create deployment group.

**Step25- Deployment group created now go for Create Deployment.**

**Step26- Click on create Deployment.**

**Step27- Provide revision type-my application is stored in s3**

- Give revision location:copy your bucket path and paste it in revision
Location.

- Revision file type .Zip

**Step28- Click on Create Deployment**

**Step29- Monitor the logs in status.**

**Step30- Copy the instance public ip and paste it in browser e.g 18.191.48.249:3000**
- Application is running with both ips

**Step31-Goto ALB and copy the dns and paste it in the browser.**
- Application is running live
- Now hit refresh and see the host changes because of Target groups serving traffic from ALB.




7.13 Understanding and Implementing Deployment Configuration -1
---
(Deployment override-Codedeploy:OneAtaTime)
----

**Step1- Goto Previously created CodeDeployment group and Click on Create Deployment.**

**Step2- Give revision location and scroll down to deployment group override**

**Step3- In deployment configuration select codeDeployDefault:oneAtatime**
- Click create deployment

**Step4- In deployment lifecycle events-- 1-instance is in progress and 2 are in Pending**
- Now 2nd instance is in progress and 3rd pending and in next step 3rd is in progress.

7.13 Understanding and Implementing Deployment Configuration -1
----
(Deployment override-Codedeploy:Custom-test)
---






7.15 Blue Green Deployment of Sample App
----

**Step1- Goto Previously created CodeDeployment group and Click on Create Deployment.**

**Step2 -Edit code deployment group and scroll down to deployment type**
- Select Blue/Green and click on save changes.

**Step3-Now click on Create Deployment and give revision Location and create deployment.**

**Step4- Monitor Lifecycle Events-**
- Provisioning replacement instances--3 of 3 replacement instances provisioned
- Installing application on replacement instances---3 of 3 instances updated
- Rerouting traffic to replacement instances--
- Terminating original instances----
- Monitor the Traffic shifting progress.

- Scroll down to see the deployment in the EC2 Instances.




















Section 8 : Deploying Sample App on AWS (With CodePipeline)
----

**8.3 Setting up ec2 Instance**
- 1. AWS Console>All services>EC2
- 2. Click on Launch Instance :
- 3. Select AMI Linux2
- 4. Choose Instance type t2 micro.
     Click Next:Configure Instance
- 5. Leave everything  default beside IAM Role and User Data Section
-    Click Create IAM Role
-    AWS Console>IAM>Role>Create Role
- 6.  Now come back to EC2 Instance creation page.
     Select IAM Role as node-sample-ap-ec2-role
- 7. Refer script for user data.
```
#!/bin/bash
yum update -y
yum install ruby -y
yum install nmap-ncat -y
yum install wget -y
cd /home/ec2-user
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
chmod +x ./install
./install auto
service codedeploy-agent status
```
- 8. Click Next:Add Storage---keep DefaultClick Next Tags in Tags give key as name and value as deploy

- 9. Configure security groups:Give All Traffic access for as of now(not recommended in production)

- 10. Click on review and Launch

- 11.Create a key pair and download it .

- 12.View Instances

8.5 Sample App Deployment through CodePipeline (For Single ec2)
---

 **Step1-AWS Console>All services>DevelopersTools>CodePipeline>Getting started**

- Click on Create pipeline

**Step2- Type pipeline name as “course-master”**
- In Service role select New Service role-check the box and it will take role name automatically 

**Step3-Code commit stage:-**
- Select custom location and S3 bucket Name.
- Encryption key -default
- Click on Next

**Step4-Select source provider as AWS Code Commit**
- Fill the Repository name as node-sample-ap,
- Branch name -master
- and change detection option- Amazon Cloud watch Events 

**Step5- Click on Next**

**Step6 -Build Stage** 
- Select Build provider as AWS code build,Select your region,project name “node-sample-ap”and build type as single build 

**Step7- Click Next**

**Step8- Deploy Stage:**
- Type deploy provider as AWS Code Deploy,
- Region-US East(Ohio),
- Application name-”node-sample-ap-deploy” and
 - Create Deployment group-node-sample-ap-group

- Click Next
- Click Create Pipeline


**Step9 -See the progress of code pipeline**
- First it will go to source stage and after that move to Build stage
- Now build is running you can check the status of build by clicking on details
- Build is successful now code pipeline will move further to Deploy stage

**Step10 -Deploy Stage:**

- You can check the status of deploy by clicking on Details.
- Deployment  is successful now.
- You can check the application URL 
- Application  is running.

**Step11- Now we will change the code and push it to code commit and after that  Code pipeline will start automatically for applying the change in code.**

**Step12- For this first open Git Bash after that open your files to edit** 
- Go to Codepipeline and see that CodePipeline is activated.
- Build is happening with the latest commit.


8.6 Sample App Deployment through CodePipeline (ec2-Fleet)
---
- Create ASG with LC and also create TG and ALB
- Now  Create pipeline for same deployed App and put ASG desired min,max value to 3 with same steps as in 8.5

8.7 Sample App Deployment through CodePipeline (For ElasticBeanstalk) 
----

**Step1-AWS Console>All services>DevelopersTools>CodePipeline>Getting started**

**Step2-Click on Create pipeline.**

**Step3--Give the source provider name as AWS CodeCommit**

**Step4--Provide build details-**
- Refer Aws Code Build

**Step5-  Provide deploy provider as Elastic Beanstalk**  
            - Select region-US East Ohio
            - Application name-newnodeproject
            -  environment-New Node Project-env

**Step6- Click on Next**

**Step7- Click on Create Pipeline.The pipeline has been created.**

**Step8-Source phase in progress**

**Step9-Source has been completed and build is in progress.**

**Step10- Build is completed and deploy is in progress.**

**Step11-Deploy has been completed.**

**Step12-   Goto elastic beanstalk and click on goto environment as status is showing healthy.**
        - See your application is running 

**8.8 CodePipeline with ElasticBeanstalk and ec2 fleet (Manual Approval)**

**Step1- refer last code pipeline of 8.7 and Click on Edit 

**Step2- Click Add stage Next To deploy**

**Step3 -Give Name of stage as “manualApproval”.Click Add stage**

**Step4- Click on Add action group in Stage created.**

**Step5 -give action name and select action provider>approval>manualapproval**

**Give name of SNS topic previously created(for sending EMail)**
- Click Done

**Step6 -click on add stage next to manaulapproval stage**

**Step7- give name as prod-deploy**

**Step8 -Click on Add action group in prod-deploy and do steps**
- Action name,action provider,region,input artifacts-source,Appl name,Dep group

**Step9 - click on save pipeline.click on release changes.**

**Pipeline will be activated automatically till approval step then approval needed sent on Email .**
- After getting approval pipeline would start to next step Prod-deploy.
- After the pipeline is completed successfully.
- Check the production environment.

###  check for AWSPipeline bucket to see the source artifacts and build artifacts






















Section 10 : Deploying Sample App With CRUD Functionality on AWS ( Without CI/CD)
----

10.2 Setting up ec2 Instance
-----

**Step1 -Setting up ec2 instance with following  IAM Role-**
- AmazonS3FullAccess
- AmazonDynamoDBfullAccess
- AmazonSSMFullAccess

**Step2- AWS Console>All Services>EC2 Dashboard>Select Instance>Actions>Connect**

**Step3- Click on Connect**

**10.4 Pushing Sample App on CodeCommit**

**Step1-**
- 1.1 AWS Console>All services>Code Commit>repositories>create repository>Create
    Give Name-MYRepo
- 1.2 Copy URL
- 1.3 Goto Local PC and open Git with Application Code location and type
```
#git init
```
```
- 1.4 #git status
```
```
- 1.5 #Git add .
```
```
- 1.6 #Git commit -m “Commit1”
```

- 1.7 # Git clone https://git-codecommit.us-west-1.amazonaws.com/v1/repos/MyRepo 
      - Provide User name and password for HTTPS Code Commit.

- 1.8 #git remote add origin https://git-codecommit.us-west-1.amazonaws.com/v1/repos/MyRepo
     - Provide User name and password for HTTPS Code Commit.
```     
- 1.9 #git push origin master
```
- 1.10 AWS Console>All services>Code Commit>repositories>MyRepo


10.5 Pushing Sample App on S3
---
**Open AWS Console>Services>S3 bucket>upload your code in zip file format**


10.6 Deploying Sample App on single ec2 
----

**Step1- Create Ec2 with this link:- Launch instance**
          -  In IAM Role give the following permissions-
          -  To see how to create IAM Role please Refer-IAM Introduction(Role)

**Step2- AWS Console>All Services>EC2 Dashboard>Select Instance>Actions>Connect**

**Step3- Click on Connect**
```sh
Step4- Run #sudo yum update
Step5- Run # sudo yum install nmap-ncat
Step6- Run # curl -sL https://rpm.nodesource.com/setup_lts.x | bash - 
Step7- Run# sudo yum install -y nodejs
Step8 -Run # sudo yum install git -y
```
Step9-Download the Zip file from S3.
        #aws s3 “BucketPath” /home/ec2-user
       ```
       #aws s3  cp s3://deploy28092020/Nodejs-curd-app-with-dynamodb.zip /home/ec2-user
       ```
Refer-Amazon S3


Change directory to ec2-user and list directory

**Step10 -     #ls**
  -  Change directory to “Nodejs-curd-app-with-dynamodb”
```
Step11 -Run #npm install
```

**Step12- Install pm2 utility-for running the application in background without keeping busy Terminal.**
```
#npm install pm2@latest -g
 #pm2 update
```
**Step14- Copy Ec2 Public IP Address and paste it in the browser**
- e.g-52.66.211.218:3000

**Step15- Open the Postman tool**

**Step17-**
             -  Click  on New Collection
             -  Name-Ec2
             -  Click on Create and create requests for-Create Table,Insert Data,read Data,update Data,Delete Item,Delete table

**Step18- Click on three dots  … >Add request**

**18.1** - Name- Create Table 
         - Save to Ec2

- Click on request created Create Table
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/createTable
- Select Body>raw>json>paste the following data.
```sh
{
    "TableName" : "Movies",
    "KeySchema": [       
        { "AttributeName": "year", "KeyType": "HASH"},
        { "AttributeName": "title", "KeyType": "RANGE" }
    ],
    "AttributeDefinitions": [       
        { "AttributeName": "year", "AttributeType": "N" },
        { "AttributeName": "title", "AttributeType": "S" }
    ],
    "ProvisionedThroughput": {       
        "ReadCapacityUnits": 1, 
        "WriteCapacityUnits": 1
    }
}
```
  
**18.2 Click on SEND**
**18.3Check the Table created in DynamoDB.** 
- Goto -AWS Console>DynamoDB>Tables>Movies(just created)

**Step19- new request for Insert Data** 
- Click on request created Insert data
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/insertData
- Select Body>raw>json>paste the following data.
```sh
{
    "TableName":"Movies",
    "Item":{
        "year": 2020,
        "title": "KGF Chapter 2",
        "info":{
            "plot": "The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now.",
            "rating": 9
        }
    }
}
```
- "New item added successfully"
- Check for added item in DynamoDB
- AWS Console>All services>DynamoDB>Tables>Items
- “Kgf Chapter 2” is added

**Step19- new request for ReadData** 
- Click on request created Read data
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/ReadData
- Select Body>raw>json>paste the following data.

**19.1 Check in DynamoDB also**


**Step20- New request for UpdateData**
- Click on request created Update data
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/updateData
- Select Body>raw>json>paste the following data.
 - AWS Console>DynamoDB>Tables>Movies>KGF Chapter2

**Step21- New request for deleteItem**
                - Click on request created deleteItem
                - Select Post in drop-down menu
                - Give URl---http://52.66.211.218:3000/deleteItem
                - Select Body>raw>json>paste the following data.


**21.1 Check in DynamoDB**

**Step22-New request for Delete Table**
                - Click on request created Delete Table
                - Select Post in drop-down menu
                - Give URl---http://52.66.211.218:3000/deleteTable
                - Select Body>raw>json>paste the following data.
- Table is Deleted.


10.7 Deploying Sample App on a ec2 fleet-1
---------

**Step1.Source code is uploaded in the repository Myrepo in AWS Commit step.**

**Step2- CodeBuild**
**2.1 AWS Console>All services>CodeBuild>Build projects>create Build project**
- Project name-DynamoDBbuild
**2.2 Source-AWS CodeCommit**
- Repository-MYRepo
- Reference Type-Branch
- Branch-master

**2.3 Environment**
- Environment image-Managed image
- Operating system-Amazon linux 2
- Runtime-Standard
- Image-standard 3.0

**2.4-Role**
- Service role-new service role
- Role name-Automatically taken
- Buildspec-Use a buildspec file

**2.5 Artifacts -**
- Type-Amazon S3
- Bucket name-”S3 Bucket Name”

**2.6 Artifacts packaging -Zip**
- Select -Disable artifact encryption

**2.7 Click Create build project**

**2.8 project created** 
     - Click on start build 

**2.9 Build Configuration**

**2.10 Source**
- Click on start build

**2.11 Build started**

**2.12 see phase details**


**2.13 check the Artifacts in S3**
- Build is completed successfully now move to Deployment

**Step3- CodeDeploy**

**3.1  AWS Console>All services>CodeDeploy>Applications>create application**
- Give name-DynamoDBbuild
- Compute platform-Ec2
- Click on Create application

**3.2 Application created-in order to create a new deployment,you must first create a deployment group**

**3.3 Give application name**
    - Give deployment group name
   
- Select service role for CodeDeploy-Demo(for S3 access)
- There is a need for a Launch Configuration and Auto scaling group for this deployment so creating the same.

**3.4**
- Deployment type-In-place
- Environment configuration-Select Amazon EC2 Auto Scaling groups


**3.5  Deployment settings-CodeDeployAllAtOnce**
- Do nothing in Load Balancer

**3.6 Deployment group created**
 - Click Create Deployment

**3.7 Give revision location(Copy it from S3 Artifacts location )**
- Revision file type-Zip

**3.8 Click on Create Deployment**

**3.9 Deployment Needs Instances for deployment**
 - Goto  AWS>Services>EC2>AutoScaling groups>select group and edit
- Editing Auto Scaling group Policy to Desired-2,Min-2,Max-2

**3.10 Goto EC2 Dashboard and see that 2 new instances are launching-**

**3.11 Goto Step 3.8 and click on create deployment**
       - Deployment started on Just launched instances.
**3.12 Monitor the deployment by Clicking on Events-View events**

**3.13 Copy the IPaddress of both the instances and paste it in the browser one by one**

**3.14 Application is running for both the instances.**
**Step 4- Open the Postman tool**

**Step 4.1-**
             -  Click  on New Collection
             -  Name-Ec2
             -  Click on Create and create requests for-Create Table,Insert Data,read Data,update Data,Delete Item,Delete table

**Step 4.2- Click on three dots  … >Add request**

**Step 4.3** - Name- Create Table 
         - Save to Ec2

- Click on request created Create Table
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/CreateTable
- Select Body>raw>json>paste the following data.
```sh
{
    "TableName" : "Movies",
    "KeySchema": [       
        { "AttributeName": "year", "KeyType": "HASH"},
        { "AttributeName": "title", "KeyType": "RANGE" }
    ],
    "AttributeDefinitions": [       
        { "AttributeName": "year", "AttributeType": "N" },
        { "AttributeName": "title", "AttributeType": "S" }
    ],
    "ProvisionedThroughput": {       
        "ReadCapacityUnits": 1, 
        "WriteCapacityUnits": 1
    }
}
```
  
**4.4 Click on SEND**
**4.5 Check the Table created in DynamoDB.** 
- Goto -AWS Console>DynamoDB>Tables>Movies(just created)

**Step 4.6 - new request for Insert Data** 
- Click on request created Insert data
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/insertData
- Select Body>raw>json>paste the following data.
```sh
{
    "TableName":"Movies",
    "Item":{
        "year": 2020,
        "title": "KGF Chapter 2",
        "info":{
            "plot": "The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now.",
            "rating": 9
        }
    }
}
```
- "New item added successfully"
- Check for added item in DynamoDB
- AWS Console>All services>DynamoDB>Tables>Items
- “Kgf Chapter 2” is added

**Step 4.7- new request for ReadData** 
- Click on request created Read data
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/ReadData
- Select Body>raw>json>paste the following data.

**Step 4.8 Check in DynamoDB also**


**Step 4.9- New request for UpdateData**
- Click on request created Update data
- Select Post in drop-down menu
- Give URl---http://52.66.211.218:3000/updateData
- Select Body>raw>json>paste the following data.
 - AWS Console>DynamoDB>Tables>Movies>KGF Chapter2

**Step 4.10- New request for deleteItem**
                - Click on request created deleteItem
                - Select Post in drop-down menu
                - Give URl---http://52.66.211.218:3000/deleteItem
                - Select Body>raw>json>paste the following data.


**Step4.11 Check in DynamoDB**

**Step4.12-New request for Delete Table**
                - Click on request created Delete Table
                - Select Post in drop-down menu
                - Give URl---http://52.66.211.218:3000/deleteTable
                - Select Body>raw>json>paste the following data.
- Table is Deleted.




10.8 Deploying Sample App on a ec2 fleet-2
-----
Step1.Source code is uploaded in the repository Myrepo in AWS Commit step.
Step2- CodeBuild
2.1 AWS Console>All services>CodeBuild>Build projects>create Build project
Project name-DynamoDBbuild
2.2 Source-AWS CodeCommit
Repository-MYRepo
Reference Type-Branch
Branch-master

2.3 Environment
Environment image-Managed image
Operating system-Amazon linux 2
Runtime-Standard
Image-standard 3.0

2.4
Service role-new service role
Role name-Automatically taken
Buildspec-Use a buildspec file

2.5 Artifacts -
Type-Amazon S3
Bucket name-”S3 Bucket Name”

2.6 Artifacts packaging -Zip
Select -Disable artifact encryption

2.7 Click Create build project

2.8 project created 
     Click on start build 

2.9 Build Configuration

2.10 Source
Click on start build

2.11 Build started
2.12 see phase details


2.13 check the Artifacts in S3
Build is completed successfully now move to Deployment

Step3- CodeDeploy

3.1  AWS Console>All services>CodeDeploy>Applications>create application
Give name-DynamoDBbuild
Compute platform-Ec2
Click on Create application
3.2 Application created-in order to create a new deployment,you must first create a deployment group

3.3 Give application name
    Give deployment group name
   
Select service role for CodeDeploy-Demo(for S3 access)
There is a need for a Launch Configuration and Auto scaling group for this deployment so creating the same.

3.4 
Deployment type-In-place
Environment configuration-Select Amazon EC2 Auto Scaling groups


3.5  Deployment settings-CodeDeployAllAtOnce
Load Balancer-Select enable load balancing and select Application load balancer
Choose target group
Click create deployment group.
3.5.1 create Load balancer and target group
AWS Console>All services>EC2>Load Balancing>load balancers>create load balancer
3.5.2 Select Application Load balancer
3.5.3 Give Name
Scheme-internet facing
IP address type-ipv4
Listeners-HTTP,3000

3.5.4 Availability zone-select vpc default and select 2 AZs
3.5.5 Select security group
3.5.6 Configure routing
Target group-new target group
Give name
protocol-HTTP
Port-3000
Click Next Register Targets
3.5.7 Click Create
3.5.8 See that Load Balancer state is in Provisioning
It Takes some time to become active


3.6 Deployment group created
 Click Create Deployment
3.7 Give revision location(Copy it from S3 Artifacts location )
Revision file type-Zip

3.8 Click on Create Deployment



3.9 Deployment Needs Instances for deployment
 Goto  AWS>Services>EC2>AutoScaling groups>select group and edit
Editing Auto Scaling group Policy to Desired-2,Min-2,Max-2

3.10 Goto EC2 Dashboard and see that 2 new instances are launching-
3.11 Check the Target Group for Healthy instances AWS>EC2>Target Groups
3.12 Goto Step 3.8 and click on create deployment
       Deployment started on Just launched instances.

3.13 Monitor the deployment by Clicking on Events-View events
3.14 Copy DNS of Application load balancer and paste it in browser
3.15 See that the application is  running-

Step4- DynamoDB-Postman
 4.1- Open the Postman tool
4.2 GUI of Postman tool
4.3- 
             Click  on New Collection
              Name-Ec2
              Click on Create and create requests for-Create Table,Insert Data,read        Data,update Data,Delete Item,Delete table

4.4- Click on three dots  … >Add request
4.5 
Name- Create Table 
Save to Ec2

Click on request created Create Table
               Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/createTable
                Select Body>raw>json>paste the following data.
                
          


{
    "TableName" : "Movies",
    "KeySchema": [       
        { "AttributeName": "year", "KeyType": "HASH"},
        { "AttributeName": "title", "KeyType": "RANGE" }
    ],
    "AttributeDefinitions": [       
        { "AttributeName": "year", "AttributeType": "N" },
        { "AttributeName": "title", "AttributeType": "S" }
    ],
    "ProvisionedThroughput": {       
        "ReadCapacityUnits": 1, 
        "WriteCapacityUnits": 1
    }
}

  
4.6 Click on SEND
4.7
Check the Table created in DynamoDB. 
Goto -AWS Console>DynamoDB>Tables>Movies(just created)
4.8- new request for Insert Data
Click on request created Insert data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/insertData
                Select Body>raw>json>paste the following data.

{
    "TableName":"Movies",
    "Item":{
        "year": 2020,
        "title": "KGF Chapter 2",
        "info":{
            "plot": "The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now.",
            "rating": 9
        }
    }
}
"New item added successfully"
Check for added item in DynamoDB
AWS Console>All services>DynamoDB>Tables>Items
“Kgf Chapter 2” is added
4.9- new request for ReadData
Click on request created Read data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/readData
                Select Body>raw>json>paste the following data.
4.10
Check in DynamoDB also
4.11 
New request for UpdateData
Click on request created Update data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/updateData
                Select Body>raw>json>paste the following data.
 AWS Console>DynamoDB>Tables>Movies>KGF Chapter2
4.12

New request for deleteItem
Click on request created deleteItem
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/deleteItem
                Select Body>raw>json>paste the following data.
4.13 Check in DynamoDB
4.14

New request for Delete Table
Click on request created Delete Table
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/deleteTable
                Select Body>raw>json>paste the following data.
Table is Deleted.










10.9 Deploying Sample App on Elastic Beanstalk
Step1- Goto AWS Console>All Services>Elastic Beanstalk>Create Application
Click on Create Application
Application name-NewApp

Step2 -Click on Create

Step3 -Click on Create a New Environment
Step4 -Choose Web server Environment
          Click on Select

Step5 -See Environment Information
Environment name- Newapp-env(Auto-fill)
Step6 -Platform
           Platform-Node.js
          Platform branch-Nodejs t2 running on 64bit Amazon Linux 2
        Platform version-5.2.2(Recommended)

Step7-
7.1 Remember the following changes that were not earlier in Zip Folder env.prod file.
#No hidden files should present in that folder
##Env prod Port-8080
###Proc file-web: npm start

7.2 Application Code
Select Upload your code>Local file>Choose File>dir.zip
Click on Create environment

Step8 -Environment Creation started.
8.1 Creating Newapp-env
8.2 Deployment completed successfully.
Step9 -Click on Environments and Click on Newapp.env
Step10 -Health is OK means Application is working fine.
        Click on Go to Environment
Step11 -After clicking on Goto environment it will open in Browser.
     See your Application is Live!!!

DynamoDB-CRUD operations-
 1.- Open the Postman tool
2. GUI of Postman tool
3.
             Click  on New Collection
              Name-Ec2
              Click on Create and create requests for-Create Table,Insert Data,read        Data,update Data,Delete Item,Delete table

4.- Click on three dots  … >Add request
5. 
Name- Create Table 
Save to Ec2

Click on request created Create Table
               Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/createTable
                Select Body>raw>json>paste the following data.
                
          


{
    "TableName" : "Movies",
    "KeySchema": [       
        { "AttributeName": "year", "KeyType": "HASH"},
        { "AttributeName": "title", "KeyType": "RANGE" }
    ],
    "AttributeDefinitions": [       
        { "AttributeName": "year", "AttributeType": "N" },
        { "AttributeName": "title", "AttributeType": "S" }
    ],
    "ProvisionedThroughput": {       
        "ReadCapacityUnits": 1, 
        "WriteCapacityUnits": 1
    }
}

  
6. Click on SEND
7.
Check the Table created in DynamoDB. 
Goto -AWS Console>DynamoDB>Tables>Movies(just created)
8.- new request for Insert Data
Click on request created Insert data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/insertData
                Select Body>raw>json>paste the following data.

{
    "TableName":"Movies",
    "Item":{
        "year": 2020,
        "title": "KGF Chapter 2",
        "info":{
            "plot": "The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now.",
            "rating": 9
        }
    }
}
"New item added successfully"
Check for added item in DynamoDB
AWS Console>All services>DynamoDB>Tables>Items
“Kgf Chapter 2” is added
9.- new request for ReadData
Click on request created Read data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/readData
                Select Body>raw>json>paste the following data.
10.
Check in DynamoDB also
11. 
New request for UpdateData
Click on request created Update data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/updateData
                Select Body>raw>json>paste the following data.
 AWS Console>DynamoDB>Tables>Movies>KGF Chapter2
12.

New request for deleteItem
Click on request created deleteItem
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/deleteItem
                Select Body>raw>json>paste the following data.
13. Check in DynamoDB
14.

New request for Delete Table
Click on request created Delete Table
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/deleteTable
                Select Body>raw>json>paste the following data.
Table is Deleted.

Section 11 : Deploying Sample App With CRUD Functionality on AWS ( With CI/CD)

11.2 Setting up ec2 Instance 
Step1 -AWS Console>All Services>EC2 Dashboard>Launch Instance
Setting up ec2 instance with following  IAM Role-
AmazonS3FullAccess
AmazonDynamoDBfullAccess
AmazonSSMFullAccess

11.3 Creating CodeBuild Project-
11.4 Building Sample App-
Step1.Source code is uploaded in the repository Myrepo in AWS Commit step.
Step2- CodeBuild
2.1 AWS Console>All services>CodeBuild>Build projects>create Build project
Project name-DynamoDBbuild
2.2 Source-AWS CodeCommit
Repository-MYRepo
Reference Type-Branch
Branch-master

2.3 Environment
Environment image-Managed image
Operating system-Amazon linux 2
Runtime-Standard
Image-standard 3.0

2.4
Service role-new service role
Role name-Automatically taken
Buildspec-Use a buildspec file

2.5 Artifacts -
Type-Amazon S3
Bucket name-”S3 Bucket Name”

2.6 Artifacts packaging -Zip
Select -Disable artifact encryption

2.7 Click Create build project

2.8 project created 
     Click on start build 

2.9 Build Configuration

2.10 Source
Click on start build

2.11 Build started
2.12 see phase details


2.13 check the Artifacts in S3
Build is completed successfully now move to Deployment

11.6 Creating CodeDeploy Application
Step1- Open the AWS CodeDeploy console at https://console.aws.amazon.com/codesuite/codedeploy/home
Get started with AWS CodeDeploy by creating your first deployment application
Click on CodeDeploy>Create Application
Step2- Enter Application name code-sample-ap-deploy in Application Configuration Section
And Choose Compute platform as EC2/On-premises
Step3- Click on Create application
It will show that application created
In the next step choose Create deployment group under deployment groups section.
Give the name “ node-sample-ap-group” in the deployment group name section.

11.8 Deploying sample App on single Ec2
Step1.CodeCommit -Source code is uploaded in the repository Myrepo in AWS Commit step.
Step2- CodeBuild
2.1 AWS Console>All services>CodeBuild>Build projects>create Build project
Project name-DynamoDBbuild
2.2 Source-AWS CodeCommit
Repository-MYRepo
Reference Type-Branch
Branch-master

2.3 Environment
Environment image-Managed image
Operating system-Amazon linux 2
Runtime-Standard
Image-standard 3.0

2.4
Service role-new service role
Role name-Automatically taken
Buildspec-Use a buildspec file

2.5 Artifacts -
Type-Amazon S3
Bucket name-”S3 Bucket Name”

2.6 Artifacts packaging -Zip
Select -Disable artifact encryption

2.7 Click Create build project

2.8 project created 
     Click on start build 

2.9 Build Configuration

2.10 Source
Click on start build

2.11 Build started
2.12 see phase details


2.13 check the Artifacts in S3
Build is completed successfully now move to Deployment

Step3- CodeDeploy

3.1  AWS Console>All services>CodeDeploy>Applications>create application
Give name-DynamoDBbuild
Compute platform-Ec2
Click on Create application
3.2 Application created-in order to create a new deployment,you must first create a deployment group

3.3 Give application name
    Give deployment group name
In tags select key--name and value---deploy 
Above tags values  were given during the creation of ec2 instances in tags section..
3.4 Choose never in AWS Systems Manager section:
3.5 In Deployment settings you can select according to your choice i am using CodeDeployDefault:Allatonce.


3.6 In Load Balancer deselect Load Balancer for as of now.(will do it later in next session)

3.7 Click on Create deployment group.

3.8 -Deployment Group created now click on Create deployment.
See the deployment settings.
Deployment group node-sample-ap-group is taken automatically
3.9 Select revision type:My Application is stored in S3
Give revision location from your s3 Build artifacts output bucket(See below.)

3.10 AWS Console>S3>Buckets>node-sample-ap-output-bucket
If you don't know creating of S3 Bucket Click on How To Create S3 Bucket:

Click on bucket open revision location >click on artifacts>copy path
Paste this path to revision location option and select .ZIP from dropdown in next row.
3.11-Click on Create Deployment
Deployment created
3.12-View events in Deployment Lifecycle Events Section.

APPLICATION STOP
DOWNLOAD BUNDLE
BEFORE INSTALL
INSTALL
AFTER INSTALL
APPLICATION START
VALIDATE SERVICE

Deployment is completed.
Check Ec2 Instance URL and test the Application.
Copy the IP Address of the Ec2-Instance and paste in the browser and Hit Enter.
Application is deployed successfully.







11.9 Deploying Sample App on ec2 fleet-1
Step1.CodeCommit-Source code is uploaded in the repository Myrepo in AWS Commit step.
Step2- CodeBuild
2.1 AWS Console>All services>CodeBuild>Build projects>create Build project
Project name-DynamoDBbuild
2.2 Source-AWS CodeCommit
Repository-MYRepo
Reference Type-Branch
Branch-master

2.3 Environment
Environment image-Managed image
Operating system-Amazon linux 2
Runtime-Standard
Image-standard 3.0

2.4
Service role-new service role
Role name-Automatically taken
Buildspec-Use a buildspec file

2.5 Artifacts -
Type-Amazon S3
Bucket name-”S3 Bucket Name”

2.6 Artifacts packaging -Zip
Select -Disable artifact encryption

2.7 Click Create build project

2.8 project created 
     Click on start build 

2.9 Build Configuration

2.10 Source
Click on start build

2.11 Build started
2.12 see phase details


2.13 check the Artifacts in S3
Build is completed successfully now move to Deployment

Step3- CodeDeploy

3.1  AWS Console>All services>CodeDeploy>Applications>create application
Give name-DynamoDBbuild
Compute platform-Ec2
Click on Create application
3.2 Application created-in order to create a new deployment,you must first create a deployment group

3.3 Give application name
    Give deployment group name
   
Select service role for CodeDeploy-Demo(for S3 access)
There is a need for a Launch Configuration and Auto scaling group for this deployment so creating the same.

3.4 
Deployment type-In-place
Environment configuration-Select Amazon EC2 Auto Scaling groups


3.5  Deployment settings-CodeDeployAllAtOnce
Do nothing in Load Balancer

3.6 Deployment group created
 Click Create Deployment

3.7 Give revision location(Copy it from S3 Artifacts location )
Revision file type-Zip

3.8 Click on Create Deployment

3.9 Deployment Needs Instances for deployment
 Goto  AWS>Services>EC2>AutoScaling groups>select group and edit
Editing Auto Scaling group Policy to Desired-2,Min-2,Max-2

3.10 Goto EC2 Dashboard and see that 2 new instances are launching-
3.11 Goto Step 3.8 and click on create deployment
       Deployment started on Just launched instances.
3.12 Monitor the deployment by Clicking on Events-View events
3.13 Copy the IPaddress of both the instances and paste it in the browser one by one
3.14 Application is running for both the instances.

Step4- DynamoDB-Postman
 4.1- Open the Postman tool
4.2 GUI of Postman tool
4.3- 
             Click  on New Collection
              Name-Ec2
              Click on Create and create requests for-Create Table,Insert Data,read        Data,update Data,Delete Item,Delete table

4.4- Click on three dots  … >Add request
4.5 
Name- Create Table 
Save to Ec2

Click on request created Create Table
               Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/createTable
                Select Body>raw>json>paste the following data.
                
          


{
    "TableName" : "Movies",
    "KeySchema": [       
        { "AttributeName": "year", "KeyType": "HASH"},
        { "AttributeName": "title", "KeyType": "RANGE" }
    ],
    "AttributeDefinitions": [       
        { "AttributeName": "year", "AttributeType": "N" },
        { "AttributeName": "title", "AttributeType": "S" }
    ],
    "ProvisionedThroughput": {       
        "ReadCapacityUnits": 1, 
        "WriteCapacityUnits": 1
    }
}

  
4.6 Click on SEND
4.7
Check the Table created in DynamoDB. 
Goto -AWS Console>DynamoDB>Tables>Movies(just created)
4.8- new request for Insert Data
Click on request created Insert data
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/insertData
                Select Body>raw>json>paste the following data.

{
    "TableName":"Movies",
    "Item":{
        "year": 2020,
        "title": "KGF Chapter 2",
        "info":{
            "plot": "The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now.",
            "rating": 9
        }
    }
}
"New item added successfully"
Check for added item in DynamoDB
AWS Console>All services>DynamoDB>Tables>Items
“Kgf Chapter 2” is added
4.9- new request for ReadData
Click on request created Read data
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/readData
                Select Body>raw>json>paste the following data.
4.10
Check in DynamoDB also
4.11 
New request for UpdateData
Click on request created Update data
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/updateData
                Select Body>raw>json>paste the following data.
 AWS Console>DynamoDB>Tables>Movies>KGF Chapter2
4.12

New request for deleteItem
Click on request created deleteItem
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/deleteItem
                Select Body>raw>json>paste the following data.
4.13 Check in DynamoDB
4.14

New request for Delete Table
Click on request created Delete Table
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/deleteTable
                Select Body>raw>json>paste the following data.
Table is Deleted.


11.11 Implementing Deployment Configuration
(Deployment override-Codedeploy:OneAtaTime)
Step1- Goto Previously created CodeDeployment group and Click on Create Deployment.

Step2- Give revision location and scroll down to deployment group override

Step3- In deployment configuration select codeDeployDefault:oneAtatime
Click create deployment

Step4- In deployment lifecycle events-- 1-instance is in progress and 2 are in Pending
Now 2nd instance is in progress and 3rd pending and in next step 3rd is in progress.
11.12 Blue Green Deployment of Sample App
Step1- Goto Previously created CodeDeployment group and Click on Create Deployment.
Step2 -Edit code deployment group and scroll down to deployment type
Select Blue/Green and click on save changes.
Step3-Now click on Create Deployment and give revision Location and create deployment.

Step4- Monitor Lifecycle Events-

Provisioning replacement instances--3 of 3 replacement instances provisioned
Installing application on replacement instances---3 of 3 instances updated
Rerouting traffic to replacement instances--
Terminating original instances----
Monitor the Traffic shifting progress.

Scroll down to see the deployment in the EC2 Instances.


Section 12 : Deploying Sample App With CRUD Functionality on AWS (With CodePipeline)


12.2 Setting up ec2 Instance
Step1 -AWS Console>All Services>EC2 Dashboard>Launch Instance
Setting up ec2 instance with following  IAM Role-
AmazonS3FullAccess
AmazonDynamoDBfullAccess
AmazonSSMFullAccess

12.3 Understanding CodePipeline Service Role
The AWS Data Pipeline console creates the following roles for you:
1.DataPipelineDefaultRole - Grants AWS Data Pipeline access to your AWS resources
2.DataPipelineDefaultResourceRole - Grants your applications access to your AWS resources




12.4 Sample App Deployment through CodePipeline (For Single ec2)
Step1- Code Commit-

Step2- CodeBuild

Step3-Code Deploy

3.1  AWS Console>All services>CodeDeploy>Applications>create application
Give name-DynamoDBbuild
Compute platform-Ec2
Click on Create application

3.2 Application created-in order to create a new deployment,you must first create a deployment group

3.3 Give application name
    Give deployment group name
   
Select service role for codedeployment.

3.4 
Deployment type-In-place
Environment configuration-Select Amazon EC2 instances
Tags-Key as Name,Value as deploy
3.5  Deployment settings-CodeDeployAllAtOnce
Do nothing in Load Balancer

3.6 Deployment group created
 Click Create Deployment
3.7 Give revision location(Copy it from S3 Artifacts location )2.13 check the Artifacts in S3
Revision file type-Zip
3.8 Click on Create Deployment
3.9 Deployment events can be seen
3.10 See Ec2 instance ip address
3.11 copy the ip in the browser and see that application is running

Step4- Create Pipeline
4.1 Goto AWS Console>All Services>Developer Tools>CodePipeline>Pipelines>Create new Pipeline

Source-
Source provider-AWS CodeCommit
Repository name-
branch-master
4.2 Build
Build provider-AWS CodeBuild
Build Type-Single
Click next

4.3 Deploy- 
Deploy provider-AWS CodeDeploy
Give region
Application name
DeploymentDBbuild

4.4 Review the Pipeline.Click on create pipeline
4.5 See the pipeline has been created successfully and it would start itself in case of any change


12.5 Sample App Deployment through CodePipeline (For ec2 Fleet)

Step1- Code Commit-

Step2- CodeBuild


Step3-

3.1  AWS Console>All services>CodeDeploy>Applications>create application
Give name-DynamoDBbuild
Compute platform-Ec2
Click on Create application
3.2 Application created-in order to create a new deployment,you must first create a deployment group
3.3 Give application name
    Give deployment group name
   
Select service role
3.4 
Deployment type-In-place
Environment configuration-Select Amazon EC2 Auto Scaling groups
To know how to create Auto scaling group.Refer-Goto AWS Console>EC2>Launch Configuration

There is a need for a Launch Configuration and Auto scaling group for this deployment.

3.5  Deployment settings-CodeDeployAllAtOnce
Do nothing in Load Balancer
3.6 Deployment group created
 Click Create Deployment
3.7 Give revision location(Copy it from S3 Artifacts location )2.13 check the Artifacts in S3
Revision file type-Zip

3.8 Click on Create Deployment
3.9 Deployment Needs Instances for deployment
 Goto  AWS>Services>EC2>AutoScaling groups>select group and edit
Editing Auto Scaling group Policy to Desired-2,Min-2,Max-2
3.10 Goto EC2 Dashboard and see that 2 new instances are launching-
3.11 Goto Step 3.8 and click on create deployment
       Deployment started on Just launched instances.
3.12 Monitor the deployment by Clicking on Events-View events
3.13 Monitor the events.
3.14 Copy the IPaddress of both the instances and paste it in the browser one by one
See that application is Running.

Step4- DynamoDB-Postman
How to Download Postman tool  See-Step16 -Download Postman tool

4.1- Open the Postman tool
4.2 GUI of Postman tool
4.3- 
             Click  on New Collection
              Name-Ec2
              Click on Create and create requests for-Create Table,Insert Data,read        Data,update Data,Delete Item,Delete table

4.4- Click on three dots  … >Add request
4.5 
Name- Create Table 
Save to Ec2

Click on request created Create Table
               Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/createTable
                Select Body>raw>json>paste the following data.
                
          


{
    "TableName" : "Movies",
    "KeySchema": [       
        { "AttributeName": "year", "KeyType": "HASH"},
        { "AttributeName": "title", "KeyType": "RANGE" }
    ],
    "AttributeDefinitions": [       
        { "AttributeName": "year", "AttributeType": "N" },
        { "AttributeName": "title", "AttributeType": "S" }
    ],
    "ProvisionedThroughput": {       
        "ReadCapacityUnits": 1, 
        "WriteCapacityUnits": 1
    }
}

  
4.6 Click on SEND

4.7
Check the Table created in DynamoDB. 
Goto -AWS Console>DynamoDB>Tables>Movies(just created)
4.8- new request for Insert Data
Click on request created Insert data
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/insertData
                Select Body>raw>json>paste the following data.

{
    "TableName":"Movies",
    "Item":{
        "year": 2020,
        "title": "KGF Chapter 2",
        "info":{
            "plot": "The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now.",
            "rating": 9
        }
    }
}
"New item added successfully"

Check for added item in DynamoDB
AWS Console>All services>DynamoDB>Tables>Items
“Kgf Chapter 2” is added
4.9- new request for ReadData
Click on request created Read data
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/readData
                Select Body>raw>json>paste the following data.
4.10
Check in DynamoDB also
4.11 
New request for UpdateData
Click on request created Update data
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/updateData
                Select Body>raw>json>paste the following data.

4.12

New request for deleteItem
Click on request created deleteItem
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/deleteItem
                Select Body>raw>json>paste the following data.
4.13 Check in DynamoDB
4.14

New request for Delete Table
Click on request created Delete Table
                Select Post in drop-down menu
                Give URl---http://52.66.211.218:3000/deleteTable
                Select Body>raw>json>paste the following data.

Table is Deleted.















12.7 Sample App Deployment through CodePipeline (For ElasticBeanstalk) -1

Step1- Goto AWS Console>All Services>Elastic Beanstalk>Create Application
Click on Create Application
Application name-NewApp

Step2 -Click on Create

Step3 -Click on Create a New Environment
Step4 -Choose Web server Environment
          Click on Select

Step5 -See Environment Information
Environment name- Newapp-env(Auto-fill)
Step6 -Platform
           Platform-Node.js
          Platform branch-Nodejs t2 running on 64bit Amazon Linux 2
        Platform version-5.2.2(Recommended)

Step7-
7.1 Remember the following changes that were not earlier in Zip Folder env.prod file.
#No hidden files should present in that folder
##Env prod Port-8080
###Proc file-web: npm start

7.2 Application Code
Select Upload your code>Local file>Choose File>dir.zip
Click on Create environment

Step8 -Environment Creation started.
8.1 Creating Newapp-env
8.2 Deployment completed successfully.
Step9 -Click on Environments and Click on Newapp.env
Step10 -Health is OK means Application is working fine.
        Click on Go to Environment
Step11 -After clicking on Goto environment it will open in Browser.
     See your Application is Live!!!

Step12 -Create pipeline
4.1 Goto AWS Console>All Services>Developer Tools>CodePipeline>Pipelines>Create new Pipeline

Source-
Source provider-AWS CodeCommit
Repository name-
branch-master
4.2 Build
Build provider-AWS CodeBuild
Build Type-Single
Click next

4.3 Deploy- 
Deploy provider-AWS Elastic Beanstalk
Give region
Application name(Created in beginning)
Env-name(Created in beginning)
Click on Next

4.4 Review the Pipeline.Click on create pipeline
4.5 See the pipeline has been created successfully and it would start itself in case of any change


DynamoDB-CRUD operations-
1.- Open the Postman tool
2. GUI of Postman tool
3.
             Click  on New Collection
              Name-Ec2
              Click on Create and create requests for-Create Table,Insert Data,read        Data,update Data,Delete Item,Delete table

4.- Click on three dots  … >Add request
5. 
Name- Create Table 
Save to Ec2

Click on request created Create Table
               Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/createTable
                Select Body>raw>json>paste the following data.
                
          


{
    "TableName" : "Movies",
    "KeySchema": [       
        { "AttributeName": "year", "KeyType": "HASH"},
        { "AttributeName": "title", "KeyType": "RANGE" }
    ],
    "AttributeDefinitions": [       
        { "AttributeName": "year", "AttributeType": "N" },
        { "AttributeName": "title", "AttributeType": "S" }
    ],
    "ProvisionedThroughput": {       
        "ReadCapacityUnits": 1, 
        "WriteCapacityUnits": 1
    }
}

  
6. Click on SEND
7.
Check the Table created in DynamoDB. 
Goto -AWS Console>DynamoDB>Tables>Movies(just created)
8.- new request for Insert Data
Click on request created Insert data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/insertData
                Select Body>raw>json>paste the following data.

{
    "TableName":"Movies",
    "Item":{
        "year": 2020,
        "title": "KGF Chapter 2",
        "info":{
            "plot": "The blood-soaked land of Kolar Gold Fields (KGF) has a new overlord now.",
            "rating": 9
        }
    }
}
"New item added successfully"
Check for added item in DynamoDB
AWS Console>All services>DynamoDB>Tables>Items
“Kgf Chapter 2” is added
9.- new request for ReadData
Click on request created Read data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/readData
                Select Body>raw>json>paste the following data.
10.
Check in DynamoDB also
11. 
New request for UpdateData
Click on request created Update data
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/updateData
                Select Body>raw>json>paste the following data.
 AWS Console>DynamoDB>Tables>Movies>KGF Chapter2
12.

New request for deleteItem
Click on request created deleteItem
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/deleteItem
                Select Body>raw>json>paste the following data.
13. Check in DynamoDB
14.

New request for Delete Table
Click on request created Delete Table
                Select Post in drop-down menu
                URl---http://alb-583710237.us-west-1.elb.amazonaws.com:3000/deleteTable
                Select Body>raw>json>paste the following data.
Table is Deleted.


12.8 Sample App Deployment through CodePipeline (For ElasticBeanstalk) -2






12.9 CodePipeline with ElasticBeanstalk and ec2 fleet (Manual Approval)

Step1-Create Pipeline for Elastic BeanStalk as in  step 12.8 
Step2-Now Select pipeline and edit>Add action to the 3rd stage (AWS CodeDeploy)
Pipeline>Edit>Edit Stage>Add action group
Step3 -give Action Name
Action Provider-Manual Approval
SNS topic-
Click Done
Step4 -Click Add stage for Ec2 prod Deployment
Provide Name-”Prod-Deploy”
Click on Add Stage
Step5-
Click on Prod-Deploy>Add action group
Provide Action Name 
Action Provider-AWS CodeDeploy
Region-
Input Artifacts-Select SourceArtifacts from sourceartifcats and buildartifacts
Application Name-
Deployment Group(Edit ASG group Size value to 2 instances for deployment of production) Refer:-Sample App deployment with CodePipeline Ec2-fleet
Click on Done
Step6- Click on Release Change and See the Pipeline Running and application is Running 
Step 7- Do some change in Repo and check for the changes in Running application.



















Section 13 : Deploying Static Website on S3 (with CodePipeline)
13.3 Setting-up S3 Bucket
1.1AWS>Services>S3>Create Bucket
How to create Bucket and make it Public and Enable versioning  
1.2 Open created bucket

13.4 Configuring S3 Bucket for Website Hosting 
Click on Bucket Properties>Static website hosting
1.3 Select Use this bucket to host a website.
Index document-index.html

13.6 Creating CodePipeline for S3 Deployment
Step2- Create Pipeline

2.1 Goto AWS Console>All Services>Developer Tools>CodePipeline>Pipelines>Create new Pipeline
#Provide Pipeline name
#Select New service role
Click Next
2.2 Source-AWS CodeCommit
See the following steps for creating source

13.5 Setting-up CodeCommit for Static Content
2.2.1  Goto AWS Console>All Services>Developer Tools>CodeCommit>Create repository
2.2.2 Give repository name- StaticS3
 and Click on Create
2.2.3 Repository Created Click on Clone URL>Clone HTTPS
  For Creating HTTPS Credentials SEE-HTTPS git credentials for AWS Code Commit
2.2.4 Copied URL
2.2.5 Open Git in your Local PC.
    Open with Git Bash from this Location
2.2.6 #git init
      #git clone “Copied from Repository URL see step 2.2.3”
   After that you need to give user name and password for HTTPS.
 SEE- HTTPS git credentials for AWS Code Commit
In my case it is given already so it is not asking here.
2.2.7 #git remote add origin “Clone URL”
2.2.8 #git status
2.2.9 #git add .
         #git commit -m “Commit statement”
2.2.10
#git push origin master
2.2.11 Check in CodeCommit>Repository>StaticS3

Come back to Step 2.2 Create pipeline
Click Next
2.3  source stage
Select source provider as AWS Codecommit
Repository name-StaticS3
Branch name-master
2.4 Skip Build stage
2.5 Deploy stage-Select Amazon S3
Select -region
Select Bucket name-
   Leave S3 object key blank
   Select the check box of Extract file before deploy.
Click next 

2.6 review The Pipeline
Click Create Pipeline
2.7 See the pipeline Running
Step3- Editing index.html 
 See the change detection by Pipeline and access static S3 endpoint
3.1 Original Website page-
3.2 open file in Local PC and edit for some change and save.
3.3 Open Git and type following commands-
 # git status
#git add index.html
#git commit -m”changing Great Game”  
#git push origin master
3.4 Check the commit in CodeCommit
3.5 Pipeline is activated for the changes.
3.6 Access the endpoint of S3 and check it.
















































              


