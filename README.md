# AWS IAM Security Lab

Hands-on AWS IAM project demonstrating users, groups, permissions, MFA, least privilege, and AWS CLI configuration.

## IAM User & Permissions Management 
### Project Overview 
This project demonstrates the implementation of AWS Identity and Access management controls using users, groups, policies, MFA, and least-privilege permissions. 

### Technologies Used
- Amazon Web Services 
- AWS IAM 
- AWS CLI 
- macOS Terminal
- AWS CloudShell
- GitHub

### Skills Demonstrated
- Identity and access management 
- IAM user administration 
- IAM group management 
- AWS managed policies
- Least-privilege access 
- Multi-factor authentication 
- AWS CLI 
- Cloud security fundamentals 

### Project Architecture 
`IAM User → Developers Group → IAM Policy → AWS Resource`

### What I Learned 
- IAM controls access to AWS resources. 
- Groups simplify permissions management. 
- Policies determine which actions identities can perform. 
- MFA provides an additional authentication layer. 
- Least privilege means providing only the permissions necessary to perform a job. 

### Implementation Steps

#### 1. Created an IAM User
- Created a dedicated IAM user named `cloud-lab-user`
- Used the IAM user instead of the AWS root account for everyday administrative tasks.

#### 2. Created an IAM User Group
- Created an IAM user group to manage permissions called `Developers`.
- Added `cloud-lab-user` to the `Developers` group.

#### 3. Assigned IAM Permissions
- Attached AWS managed policies, `AmazonS3ReadOnlyAccess`, to the `Developers` group.
- Verified that cloud-lab-user inherited permissions through membership in the `Developers` group.

#### 4. Configured Multi-Factor Authentication
- Enabled MFA to add an additional layer of security to the AWS account.

#### 5. Reviewed IAM Security Settings
- Reviewed IAM users, groups, permissions, and security credentials.
- Applied the principle of least privilege by limiting access to required permissions.

#### 6. Installed and Verified AWS CLI
- Installed AWS CLI Version 2 on macOS.
- Verified the installation from Terminal using:
  
```bash
aws --version
