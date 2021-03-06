# Notes 2: Cloud Economics, Billing & Support

### Paying for AWS
- Pay as you go : Only pay for the services you use. This allows you to scale and meet demands; allows you to adapt to business needs without overcommitting budgets. 
- Save when you reserve: For certain services like EC2 and RDS, you can invest in reserved capacity. The larger the upfront payment, the greater the discount. 
- Pay less when you use more: The more you use services such as S3 and data transfer out EC2, the less you pay per GB. 

### Key Principles of Pricing 
- Understanding the fundamentals of pricing : Drivers of cost are storage, compute, and outbound data transfer.

### Start early with cost composition :
- "Managing cost-effectively from the start ensures that managing cloud investments doesn’t become an obstruction as you grow and scale."

### Pricing models : 
- __On demand__ : pay for compute or database capacity without longterm commitments and upfront payments. 
- __Dedicated instances__ : EC2, run in a VPC that on hardware that is dedicated to a single consumer. 
- __Spot instances__ : EC2, Purchase spare consuming capacity without upfront commitment and at discounted hourly rates. 
- __Reservations__ : Paying for capacity ahead of time allow you to receive a discount up to 75%. 

### Amazon Free Tier 
- Allows you to test drive some AWS features with restrictions for free. 

### Some Services free of charge 
- VPC, IAM, Elastic Beanstalk, Cloudformation 

### What is IT Infrastructure ? 
- Components required to operate and manage IT systems. The compenents include: software (applications, OS), hardware (servers, datacenters, computers...), Networking (internet, firewalls, security). 

### Total Cost of Ownership: 
-  direct and indirect costs and benefits related to the purchase of any IT component. " The goal is a final figure that will reflect the true purchase price, all things considered." 

### AWS Organizations 
- a account management service that enables the consolidation of multiple AWS accounts into an organization that you create and manage. Also includes account management and  billing capabilities of all accounts which allows you to keep a better eye on budgets, security, and compliance needs of your business. 

### Steps to create na organization 
- To create an organization, you create one of the member accounts in your organization and invite the other account. Then you use the allow list technique to delegate administors that monitor specific actions and services. 

### Limits of organizations
- guidelines for names that you create in AWS Organizations: They must be composed of Unicode characters and they must not exceed 250 characters in length. 

### Facts that I learned 
- Amazon offers free access to some services with limitations. This is useful for a consumer because they can just feel it out and have no commitment. 
- AWS also offers pay less when you use more. This is important because if consumers need more GB's, they are saving in the long run wtih AWS. 
