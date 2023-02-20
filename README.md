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





