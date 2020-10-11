# Notes 4: Cloud Secuirty with DevOps
### What is Cybersecurity?
- Protecting networks, devices, and data from unauthorized access or criminal use and the practice of ensuring confidentiality, integrity, and availability of information. 
### Poor Cybersecurity Risks: 
- malware erasing your entire system, an attacker breaking into your system and altering files, an attacker using your computer to attack others, or an attacker stealing your credit card information and making unauthorized purchases. 
### What can you do to improve your cybersecurity?
- Use strong passwords, install a firewall, multifactor authentication, etc. 
### AWS responsibility “Security of the Cloud”
- Physical security of data centers with controlled, need-based access; located in nondescript facilities, with 24/7 security guards; two-factor authentication, etc.
- Hardware infrastructure
- Software infrastructure
- Network infrastructure
### Customer responsibility “Security in the Cloud”
- The customer is responsible for what is implemented by using AWS services and for the applications that are connected to AWS. The security steps that you must take depend on the services that you use and the complexity of your system. Customer responsibilities include selecting and securing any instance operating systems, securing the applications that are launched on AWS resources, security group configurations, firewall configurations, network configurations, and secure account management.
### What is Identity and Access Management? (IAM) 
- AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources for your users. You use IAM to control who can use your AWS resources (authentication) and what resources they can use and in what ways (authorization). Authorization is the process of determining what permissions a user, service or application should be granted.
### Features of IAM 
- Shared access to your AWS account: You can grant other people permission to administer and use resources in your AWS account without having to share your password or access key.
- Granular permissions: You can grant different permissions to different people for different resources.
- Secure access to AWS resources for applications that run on Amazon EC2: You can use IAM features to securely provide credentials for applications that run on EC2 instances
- Free to use
### Essential Elements of IAM
- An IAM user is a person or application that is defined in an AWS account, and that must make API calls to AWS products.
- An IAM group is a collection of IAM users. You can use IAM groups to simplify specifying and managing permissions for multiple users.
- An IAM policy is a document that defines permissions to determine what users can do in the AWS account.
- An IAM role is a tool for granting temporary access to specific AWS resources in an AWS account. 
### Four Ways to use IAM: 
- Management console 
- AWS Command Line tools 
- SDK 
- HTTPS API
### Securing Accounts: 
- AWS Key Management Service (KMS): makes it easy for you to create and manage cryptographic keys and control their use across a wide range of AWS services and in your applications. 
- Amazon Cognito lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily
- AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS.
 ### Securing Data
- Data at rest is any information that is stored on a disk, tape or any medium in which it is not moving from system to system
- Data in Transit refers to any data that is moving across a network. Encryption of this information is accomplished by using Transport Layer Security (TLS) 
- In recent years, some of the security breaches of data have actually come from improperly configured Simple Storage Service (S3) buckets where the information was setup to be public.
### Ensuring Compliance
- compliance means conforming to a rule, such as a specification, policy, standard or law.
- AWS Config  is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources. 
- AWS Artifact is your go-to, central resource for compliance-related information that matters to you. It provides on-demand access to AWS’ security and compliance reports and select online agreements. 
### Quotes I found interesting: 
- "AWS is responsible for protecting the infrastructure that runs all of the services offered in the AWS Cloud."
- "The principle of least privilege is an important concept in computer security. It promotes that you grant only the minimal user privileges needed to the user, based on the needs of your users"
### Facts I learned: 
- keeping software up to date is key in maintaining your computer's security. Installing software patches so that attackers cannot take advantage of known problems or vulnerabilities. 
- Responsibility of security is shared between AWS and the customer alike. AWS is responsible for providing infrastructure. The customer is responsible for purchasing accurate security meaures and ensuring that the correct people have access. 
