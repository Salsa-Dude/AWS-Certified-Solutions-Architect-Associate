## Identity Access Management & S3

#### IAM 101
- IAM (Identity Access Management) allows you to  manage users and their level of access to the AWS console. 
- It is important to understand IAM and how it works, both for the exam and for administering a company’s AWS account in real life. 

#### Identify Access Management (IAM) offers the following features: 

- Centralised control of your AWS account
- Shared Access to your AWS account
- Granular permissions
- Identity Federation (including active directory, facebook, linkedin, etc)
- Multi Factor Authentication
- Integrates with existing active directory accounts allowing single sign-on.
- Provide temporary access for users/devices and services where necessary
- Allows you to set up your own password rotation policy.
- Integrates with many different AWS services 
- Supports PCI DSS compliance (framework)
- Offers fine-grained access control to AWS resources.

#### Key Terminology for IAM
- Users - End users such as people, employees of an organization
- Groups - A collection of users. Each user in the group will inherit the permissions of the group. 
- Policies - are made up of documents, called policy documents. These documents are in a format called JSON and they give permissions as to what a User/Group/Role is able to do.
- Roles - You create roles and then assign them to AWS resources.

#### Exam Tips
- IAM is Universal. It does not apply to regions at this time
- The “root account” is simply the account created when first setup your AWS account. It has complete Admin access.
- New users have NO permissions when first created
- Default level of access of a newly created IAM user is no access to any AWS service.
- New users are assigned Access Key ID & Secret Access Keys when first created
  - These are not the same as a password. You cannot use Access Key ID & Secret Access Key to log in to the console. You can use this to access AWS via the API and Command Line, however. 
  - You only get to view these once. If you lose them, you have to regenerate them. 
- Always setup Multi Factor Authentication on your root account.
- You can create and customise your own password rotation polices. 
- Power User allows Access to all AWS services except the management of groups and users within IAM. Special role used for users that need to administer resources, but you do not want them to mess with permissions.
- To access the console you use an account and password combination. To access AWS programmatically you use a Key and Secret Key combination


