# Notes 6: Compute

### What is an Operating System? 
- An operating system is the most important software that runs on a computer. It manages the computer's memory and processes, as well as all of its software and hardware. It also allows you to communicate with the computer without knowing how to speak the computer's language. Without an operating system, a computer is useless. 
### What is an OS' job? 
- Other than managing the computer's hardware and software... The OS coordinates access to the computer's CPU, memory, and storage to ensure the program gets what it needs. 
### Types of OS
- Windows, Macintosh, Linux. All use GUI (Graphic User Interface) which uses a mouse and icons. 
## AWS Compute Services 
### Virtual Machines 
- Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. This allows you to build Infrastructure as a Service (IaaS) applications for instance-based virtual machines. 
### Serverless 
- AWS Lambda lets you run code without provisioning or managing servers. You pay only for the compute time you consume—there is no charge when your code is not running.
### Containers 
- AWS offers many different container services such as Amazon Elastic Container Service, Amazon Elastic Kubernetes Service, AWS Fargate, and Amazon Elastic Container Registry. These services are instance-based and enable you to run multiple workloads on a single OS. Containers spin up more quickly than virtual machines, thus offering responsiveness.
### Platform as a Service
- PaaS allows a company to focus on coding and making apps rather than managing infrastructure. AWS Elastic Beanstalk provides PaaS. It facilitates the quick deployment of applications that you create by providing all the application services that you need.
### Important Services and what the do: 
- EC2 Provides resizable virtual machines. 
- AWS Lambda is a serverless compute solution. You pay only for the compute time that you use. 
- AWS Elastic Beanstalk provides a simple way to run and manage web applications.
### Instances 
- virtualized servers, allowing you to change their capabilities with a button. At AWS, these virtual server instances come in different families and sizes, and they offer a wide variety of capabilities. 
- A method of OS virtualization that allow you to run an application and its dependencies in resource-isolated processes. AWS Fargate. 
### Functions 
- abstract the execution environment from the code you want to execute. AWS Lambda. 
### What is a VM ?
- A VM is a software-based computer that exists within another computer’s operating system, often used for the purposes of testing, backing up data, or running SaaS applications. 
### What is a Hypervisor? 
- A hypervisor is a piece of software, firmware, or hardware that VMs run on top of. The hypervisors themselves run on physical computers, referred to as the “host machine”. The host machine provides the VMs with resources, including RAM and CPU. 
### What are VM's used for ? 
- Testing, running software designed for other OS's, running outdated software. 
### How does cloud computing use virtual machines?
- Running SaaS applications
- Backing up data
- Hosting services like email and access management
### What is EC2 
- Amazon Elastic Compute Cloud (EC2) forms a central part of AWS by allowing users to rent virtual computers on which to run their own computer applications. EC2 encourages scalable deployment of applications by providing a web service through which a user can boot an Amazon Machine Image (AMI) to configure a virtual machine, which Amazon calls an instance, containing any software desired. 
### Instance Types 
- The first letter T is the family name of the instance type, the famly name
- The number after the letter is the generation number, so a T3 is the third generation in the T family
- The last part after the period, is the size of the instance, which is a large
- Instance types vary in several ways, including: CPU type, CPU or core count, storage type, storage amount, memory amount, and network performance.
### AMI
- Pre-configured virtual machines with an ever-growing list of operating systems. These can help you get started faster and launch multiple instances from a single AMI.
### EC2 Pricing
- On demand :  you pay for compute capacity by per hour or per second depending on which instances you run. No longer-term commitments or upfront payments are needed.
- Spot instance: Request spare Amazon EC2 computing capacity for up to 90% off the On-Demand price. Amazon EC2 Spot instances are spare compute capacity in the AWS cloud available to you at steep discounts compared to On-Demand prices. 
- Per-second : you pay for only what you use. It takes cost of unused minutes and seconds in an hour off of the bill, so you can focus on improving your applications instead of maximizing usage to the hour. Especially, if you manage instances running for irregular periods of time, such as dev/testing, data processing, analytics, batch processing and gaming applications, can benefit.
### Cost Optimization 
- Right Pies: Choose the right balance of instance types and ensure that what you provision matches what you need.
- Increase elasticity: Traditional IT costs and hardware requirements are tailored for peak usage and are rarely turned off. In the cloud, you can optimize cost to meet dynamic needs and turn resources off when they are not needed.
- Leverage the right pricing model: AWS provides a range of pricing models that can be combined to optimize pricing based on current or forecasted capacity needs. Choose the right pricing model to optimize costs based on the nature of your workload and usage patterns.
- Optimize storage: AWS provides multiple storage tiers at prices designed to meet performance. You can pick and choose which method of storage will reduce the most cost. 
### Advantges of Cloud Computing
- The Consistency in Cloud Storage: The container enhances portability. It eliminates the organizational and technical frictions so that the program moves through the entire process cycle. 
- Application Version Control: Through container in cloud computing, the users can look on the current version of the application code as well as their dependencies.
- Efficiency in the Operational Activities: The users can achieve more resources through the container in cloud computing. 
- Productivity of the Developers: The containers deduct the dependencies and conflicts between the cross-service and thus the productivity increases.
### What are Docker and Kubernetes?
- Docker: A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.
- Kubernetes:  portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. 
- Differences: Kubernetes is meant to run across a cluster while Docker runs on a single node.
### Serverless Computing: 
- Serverless computing is a method of providing backend services on an as-used basis. Serverless architecture allows users to write and deploy code without the hassle of worrying about the underlying infrastructure. Serverless computing allows developers to purchase backend services on a flexible ‘pay-as-you-go’ basis, meaning that developers only have to pay for the services they use. The frontend is the part of the application that users see and interact with, such as the visual layout. The backend is the part that the user doesn’t see; this includes the server where the application's files live. 
### Quotes I found Interesting: 
- "Virtual hardware’ may sound like a bit of an oxymoron, but it works by mapping to real hardware on the host computer."
- "This guest machine contains both the application and whatever it needs to run that application (e.g. system binaries and libraries)."
### Facts I learned : 
- A hypervisor is a piece of software, hardware, or firmware that VMs run on top of. The computers they run on are referred to as "host computers" 
- You can have two or more OSes running on one computer. In virtualization, a piece of software behaves as if it were an independent computer. This piece of software is called a virtual machine, also known as a ‘guest’ computer. 

