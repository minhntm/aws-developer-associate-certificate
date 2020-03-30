# IAM

## IAM is consist of:

- Users
- Groups
- Roles

![IAM/Untitled.png](images/iam.png)

- IAM is global
- IAM has many predefined "managed policies" by Amazon
- Can integrate users with IAM, so employee can login into AWS using company credentials by using **Identity Federation** (Eg: company use Active Directory, SAML standard)

## Security Tips:

- use MFA (Multi Factor Authentication)
- give users the minimal amount of permissions they need to perform their job
- 1 IAM User per 1 Physical Person
- 1 IAM Role per Application
- never share IAM credentials
- never write IAM credential in code or commit to git
- only use the ROOT account for initial setup
- never put personal credentials on EC2 ⇒ use IAM roles in stead