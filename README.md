# AWS-Certified-Developer-Associate-keypoint

## IAM 
IAM = Identity and Access Management
IAM permission: user or groups can assigned JSON documents called policies
Key: Least Privilege principle (don't give more permissions than user needs)

## IAM policies structure:
1. Version
2. Id
3. Statement{
4. -Sid statement Id
5. Effect (allow,deny)
6. principal: policy apply to which role
7. Action:Action allow or deny
8. Resource: resource user can use
9. Condition:when to apply the effect
}

## password policy
Strong passwords (minimum password length, specific character types, upper lower etc)
Allow user change own password, require user change pwd some time(expiration)
prevent pwd re-use

## MFA -  multi factor authentication
pwd + security device
google authenticator
authy
universal 2nd factor security key (U2F)

## 3 way to access AWS
1. AWS management console
2. AWS Command Line Interface (CLI)
3. AWS Software Developer Kit (SDK)

## Cloudshell

terminal online
cli:
aws iam list-users
aws --version
cloudshell do not available in all region

## IAM Security Tools
IAM credential report(account-level)report with all accounts and its credentials
IAM Access Advisor(user-level)Access advisor show service permission granted to a user and when services were last accessed

## IAM best practices
1. Don't use root account except setup
2. don't borrow others credentials(NEVER!)
3. Assign users to groups and sasign permission to groups
4. create strong password policy
5. use MFA
6. create use Roles for giving permissions to AWS services
7. Use Access Keys for Programmatic access (CLI/SDK)
8. IAM Credentials report for Audit permission

## EC2
EC2 = elastic compute cloud = infrastructure as a service
rent virtual machine EC2
Store data on virtual drives EBS
Distributing load accross machine ELB
Scaling service using auto-scaling group ASG

OS: Mac,Linux, Windows
configuration
compute power & core(CPU)
random-access memory(RAM)
Space: EBS & EFS
hardware: EC2 Instance
Network card: speed, IP
Firewall rules: security group
Bootstrap script:EC2 User Data
bootrstrap : only run once when machine starts


## EC2 instance types
M5.2xlarge
M: instance class
5: generation (improves over time)
2xLarge:size within the instance class

## security groups
Firewall rules -> ip/port
sg live outside the EC2 so EC2 won't know what happened
not acceessible(timeout) is security group issue, but connection refused is application error

## classic ports
22= SSH secure shell - log into linux instance
21 = FTP file transfer protocol - upload file into a file share
22 = SFTP Secure file transfer protocol (FTP+SSH)
80 = HTTP 
443 = HTTPS
3389 = RDP(remote desktop protocol) log into windows

## SSH Summary

SSH=[MAC,Linux,Windows>=10]
Putty=[allWindows]
EC2 Instance Connect = [Mac, Linux, Windows]

## Purchasing options

On demand instances - pay by second (highest cost, no upfront payment)
reserved
reserved Instances - 72% to ondemand
convertible reserved instances - 66% can change instance type, instance family, OS Tenancy
saving plan -72% instance size, OS, tenancy
spot instances -90% may lose (cost-efficient) can do batch jobs, data analysis, image processing, distributed workloads
Dedicated host - physical server capacity fully dedicated to your use (compliance requirements, use existing server-bound software licences) most expensive option, (bring your own licence, strong regulatory or compliance needs)
dedicate instances - may share hardware with other instances,no control over instance placement
capacity reservations - reserve on demand instances capacity in specific AZ for any duration, no time commitment and no billing discounts, fit for short-term unintrerrupted workloads need be in specific AZ

### summary
On demand:coming and staying in resort whenever we like, we pay full price
reserved: like planning ahead and if plan stay for a long time, may get a good discount
saving plan: pay certain amount, and change room type
spot instances: most discount, but kicked out at any time
dedicated host: book entire building
capacity reservation: book room pay full price even don't stay in















