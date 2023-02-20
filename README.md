# AWS-Certified-Developer-Associate-keypoint

## IAM 
IAM = Identity and Access Management
IAM permission: user or groups can assigned JSON documents called policies
Key: Least Privilege principle (don't give more permissions than user needs)

## IAM policies structure:
1. Version
2. Id
3. Statement
4. -Sid statement Id
5. Effect (allow,deny)
6. principal: policy apply to which role
7. Action:Action allow or deny
8. Resource: resource user can use
9. Condition:when to apply the effect

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


