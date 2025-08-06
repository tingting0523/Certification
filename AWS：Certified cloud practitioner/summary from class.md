**1.What is Cloud Computing and Services?In your own words, what do you think Cloud computing is? and its associated services?**  
Cloud computing refers to the use of remote servers hosted on the internet to store, manage, and process data, instead of using a local server or a personal computer. These services include data storage, servers, databases, networking, software, analytics, artificial intelligence.  
  
**2.What's the different between Public, Private cloud and Hybrid? State the differences between these types** 
Public cloud means everything built on the cloud.  
Private cloud means everything built on company’s data centers also known as on-Premise.  
Hybrid means using both on-Premise and a cloud service, like you have a connection between your on-premise environment and public cloud.  
  
**3.What's the benefit of the cloud?**
Agility, Pay as you go pricing, Economy of scale, Global Reach, Security, Reliability, High Availability, Scalability, Elasticity, Fault Tolerance, Disaster Recovery  
  
**4.What is AWS Infrastructure? Explain?**
The AWS Global Infrastructure is globally distributed hardware and data centers that are physically networked together to act as one large resource for the end customer. The Global Infrastructure include:  
a.Regions: geographically distinct locations. Every region is physically isolated from every other region in terms of location, power, water supply. If the power goes out, it is not going to affect the other regions.  
b.Availability Zones: the physical location made up of one or more datacenter. AZs is one or more physical isolated data centers in AWS regions. Generally a region consist of three availability zones.  
c.Fault Tolerance: the ability of a system—whether it's hardware, software, or a network—to continue operating properly even if part of the system fails. It ensures high availability, reliability, and continuous service, even in the event of hardware or software malfunctions.  
d. Point of Presence: a connection between AWS region and the end user for content caching and fast transfer. It include Edge Locations and Regional Edge Caches / Locations. Edge Locations cache the most frequently visited content. Regional Edge Caches / Locations caches are not very popular but still have access needs.  
e. Local Zones: data centers located very close to a densely populated area.  
f. Wavelength Zones: mainly for edge computing, associated to 5G networks. Applications will have ultra-low latency being as close as possible to the users.  
f. Data Residency: The enterprise's data must be stored in a specific geographical location or country to meet data compliance and control.    
g. Sustainability: include renewable energy, cloud efficiency, water stewardship.   
h. AWS Ground Station: a fully managed ground station service.  
i. AWS Outposts: a fully managed service that offers the same AWS infrastructure and AWS Services APIs tools. So on and so forth. That is similar to their Cloud portal, but instead, instead of AWS, hosting the hardware and managing all of that. They will send you the rack with the servers in it, and then you manage your data and everything from the AWS portal while having and maintaining the actual. Hardware from AWS within your data center.  
  
**5.What are the differences between Regional and Global?**  
Regional only have certain permissions in a specific region.  
Global means no regional restrictions  
  
**6.What is the AWS Availability Zone?**  
The physical location made up of one or more datacenter.  
AZs is one or more physical isolated data centers in AWS regions. Generally a region consist of three availability zones.   
  
**7.Define and explain the following tools within AWS console below:**  
**CLI**：AWS Command Line Interface, an open-source tool that enables you to control multiple AWS services from the command line and automate them through scripts.     
**CloudShell**: a brower-based shell that is built in within the AWS Management console. It include one free gigabyte storage, and after that, you have to pay for everything. It support scripting command line and programming.  
**SDK**: Software Development Kit, a collection of tools and services that developers utilize, and it's all come up in one installable package.   
**ARN**: Amazon Resource Name, Amazon Resource Names (ARNs) uniquely identify AWS resources. ARNs are required to specify a resource unambiguously across all of AWS.     
**IaC**：Infrastructure as code, a tool that will allow us to write a configuration script so it can automate create, update, or destroy our cloud infrastructure.     

  
**8.What's AWS Cloud Architecture Terminology?**  
**Availability**: Your ability to ensure a service remains available eg. Highly Available (HA). High availability depends on Elastic Load Balancer（ELB）, it allows you to evenly distribute traffic to multiple servers, and one or more data center or availability zone. If one of the data center or availability zones become unhealthy, then it will balance the load across the other available data center. It will shift the traffic automatically from the affected.  
**Scalability**: Your ability to grow rapidly or unimpeded. Ability to increase your capacity based on the increase of demand for the traffic. It include Vertical scaling/scaling up and Horizontal scaling/scaling out. When you want to run processes better, so you can use Vertical scaling to increase or upgrade your server. When a lot of people coming, so you can use Horizontal scaling to create duplicate of the same configuration of that instance.  
**Elasticity**: Your ability to shrink and grow to meet the demand. High elasticity depends on Auto Scaling Groups (ASG), it allow you to automatically add or remove servers based on the scaling rule.  
**Fault Tolerance**: Your ability to prevent a failure. Service remains available or remain active. Service to ensure there is no single point of failure, preventing any failure from happening.  
**Disaster Recovery**: Your ability to recover from a failure eg. Highly Durable (DR). How quickly you can revert back. High durability is the ability to recover from a disaster and mainly prevent the loss of data.  
  
**9.What are the different computing services within AWS? Highlight 4 services and explain their use.**
**1.Elastic Compute Cloud (EC2)**： a web service that provides resizable compute capacity in the cloud. It allows you to run virtual machines (instances) on-demand. Used for Host scalable web applications, Run backend processing systems, Customize instance type, storage, and network settings, and Use Auto Scaling and Load Balancing to handle traffic changes.  
**2.Amazon LightSail**：a simplified cloud platform with pre-configured environments for websites and web applications, ideal for developers who want easy setup and low management overhead. Used for Launch websites, blogs (e.g., WordPress), and simple web apps, Use pre-packaged development stacks (LAMP, Nginx, Node.js), Includes fixed pricing and bundled storage, compute, and networking.  
**3.Elastic Container Service (ECS)** ：a fully managed container orchestration service that allows you to run and scale containerized applications using Docker. Used for Deploy containers on EC2 or AWS Fargate, Automate service discovery, load balancing, and scaling, and Integrate with CI/CD pipelines for modern app development.  
**4.Elastic Container Registry (ECR)** ：a fully managed Docker container registry that allows you to store, manage, and deploy container images securely. Used for Push and pull container images for use with ECS, EKS, or EC2, Secure images with AWS IAM permissions and encryption, and Integrate with build pipelines for automated image publishing.  
  
**10.What are the different types of storage services? Highlight at least 3.**
**1.Elastic Block Store (EBS)**：Block  
**2.AWS Elastic File Storage (EFS)**：File  
**3.Amazon Simple Storage Service (S3)**：Object  
  
**11.What is AWS Shared Responsibility? and its Model? Explain the differences!**
The AWS Shared Responsibility Model is a security and compliance framework that defines which responsibilities are handled by AWS (the cloud provider) and which are handled by you (the customer) when using AWS services. The AWS shared responsibility model helps organizations that adopt the cloud to achieve their security and compliance goals.  
Customers are responsible for Security in the Cloud. AWS is responsible for Security of the Cloud.  
  
**12.What are the following AWS services below?**
**VPC**  
**EC2**  
**Route 53**  
**RDS**  
**S3**  

  
**13.What's the difference between a Dedicated and Spot on EC2?**

  
**14.What's the difference between On-Demand and Reserved EC2?**

  
**15.What's the difference between VMs and Containers?**

  
**16.Explain What is AWS Identity and Access Management (IAM)? Explain!**

  
**17.What's the difference between the following AWS services below:**  
**Cloudfront**  
**Cloudwatch**  
**Cloudtrail**  

  
**18.What is AWS Elastic Beanstalk?**   

  
**19.What does serverless mean?**  

  
**20.What's the difference between the following services below:**  
**AWS Explorer**   
**AWS Cost and Management**   
**AWS Price Calculator**  

  
**21.What is AWS Well Architected Framework? Explain!**  

  
**22.What's the difference between the following services below and what they do?**  

  
**23.AWS Inspector vs Artifact**  

  
**24.AWS Guarddurty vs AWS Config**  

  
**25.AWS Shield vs AWS Macie**  

  
**26.What are AWS support plans?**  
**27.How can you get a Technical Account Manager (TAM)?**  
