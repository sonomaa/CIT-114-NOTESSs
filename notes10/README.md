# Notes 10: Automatic Scaling & Monitoring

### Planning for Scale and Resiliency
- “capabilities can be elastically provisioned and released” describes a situation in which a hosted cloud application can seemingly be changed on demand to provide the desired level of performance by adding performance or taking away the level of performance.
-  For applications hosted in the cloud that need to be able to handle more users or additional queries at a moment’s notice, automated scale is the goal, and it’s one that can be accomplished using built-in AWS management services.

### THE CONCEPT OF MONITORING
- You can add your own third-party monitoring solution’s monitoring agent to your EC2 instances. You don’t have to use CloudWatch; you might have specific needs and requirements that CloudWatch can’t match.
- Auto scaling with CloudWatch alarms—Automatically adjust your applications based on need with EC2 auto scaling, ELB, and CloudWatch alarms.
- Billing alarms enabling you to monitor costs—Control costs by matching billing alerts to actual budget targets using billing alerts and SNS notifications.

### WHAT IS CLOUDWATCH
- CloudWatch is a monitoring service embedded in the AWS cloud operating system. Many AWS services use CloudWatch to collect metrics that you can use to analyze how your service is currently operating.
#### Monitoring
- Basic monitoring provided by CloudWatch is free of charge and, depending on the AWS service, a select number of metrics are enabled. Metrics report to CloudWatch on a variety of intervals. There is no default among all the services that are supported.
#### Logging
- CloudWatch also has a logging service that allows you to send your log data from your Linux and Windows instances to CloudWatch log groups. This enables you to further analyze and search your log data for any specific patterns, such as errors or system issues. 
### CLOUDWATCH TERMINOLOGY
- Namespace—Each AWS service stores its CloudWatch metrics and associated data in its own container. 
- Units of measurement—Statistics are defined by bytes, seconds, count, or percentage.
- Alarms—An alarm starts an action based on the state of the metric’s data over the defined time. Alarms can be notifications using SNS topics, an EC2 action, or an auto scaling action. 
### ELASTIC LOAD BALANCING SERVICES
- provides a level of redundancy; if one server in the cluster of servers being load-balanced fails, the application or service is still available.
### APPLICATION LOAD BALANCER (ALB)
-  The AWS ALB is designed for the load balancing of containers, instances, and private IP addresses using target groups. A target group is the destination where the listener sends incoming requests. Targets include instances, containers, and IP addresses.
### CONFIGURING HEALTH CHECKS
- Health checks can be configured for each target group against the registered targets. health checks ensure your resource is available and ready to accept user requests.
### NETWORK LOAD BALANCER
- designed for supporting private resources using the TCP protocol and port number at the fourth layer of the OSI stack. 
### LAUNCH TEMPLATES
- A launch template is similar to a launch configuration, with the added feature of versioning. 
### AWS AUTO SCALING 
- This version is a management tool for scaling across application stacks using the familiar ELB service for load-balanced distribution of EC2 compute instances

### Fact I learned: 
-  behind the scenes, ELB is actually a large redundantly hosted regional service that can scale on demand. 
-   ELB monitors each online load balancer and scales the capacity required based on the incoming requests.
### Quotes I found Interesting: 
- "One of the best example of AWS service integration and automated problem-solving is the relationship between the gang of three essential AWS services: CloudWatch, Auto Scale, and ELB (load-balancing), which can work together seamlessly."
- " Remember: all AWS resources have defined soft limits that limit the number of AWS resources that are available to you as an AWS customer."
