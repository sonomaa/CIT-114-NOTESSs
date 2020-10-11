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
