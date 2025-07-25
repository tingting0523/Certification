1. Which of the following is a serverless compute offering from AWS? !
    - A. AWS SQS
    - B. AWS SNS
    - C. AWS Lambda
    - D. AWS EC2          

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  C 
    </details>

2. Which of the following storage mechanisms can be used to store messages effectively which can be used across distributed systems. ! 
    - A. Amazon EBS Snapshots  
    - B. Amazon EBS Volumes
    - C. Amazon SQS
    - D. Amazon Glacier        

    <details markdown=1><summary markdown='span'>Answer</summary>  
      Correct answer:  C     
    </details>

Amazon SQS (Simple Queue Service) 是一种完全托管的消息队列服务，专门设计用于**跨分布式系统**可靠地存储和传递消息。它支持异步通信，解耦应用组件。  
Amazon EBS Volumes 和 EBS Snapshots 是块存储和其备份机制，主要用于持久存储磁盘数据，**不适合消息传递**。  
Amazon Glacier 是冷数据归档存储，适合长期存储数据，不适合实时消息处理。  
  
3. Which one of the following features is included in all AWS Support plans?  
    - A. A dedicated support person  
    - B. A technical Account Manager
    - C. 24/7 access to Customer Service     
    - D. Access to all features in the Trusted Advisor  

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:   C
    </details>

4. You are are running a web-application and you want to improve response times for data that is requested frequently. Which AWS service should you use to improve performance to frequently accessed data?  
    - A. Amazon DynamoDB     
    - B. Amazon RDS
    - C. Amazon ElastiCache   
    - D. Amazon Simple Object Storage

    <details markdown=1><summary markdown='span'>Answer</summary>  
      Correct answer:  C   
    </details>

5. A company wants to utilize AWS storage. For them, low storage cost is paramount, the data is rarely retrieved, and data retrieval times of several hours are acceptable for them. What is the best storage option to use?  !
    - A. AWS CloudFront     
    - B. EBS-backed storage connected to EC2  
    - C. AWS Glacier     
    - D. AWS S3 Reduced Redundancy Storage

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:   C
    </details>

AWS Glacier 是一种专为长期归档和备份设计的存储服务，成本非常低，但数据检索通常需要数小时，适合访问频率极低且对检索时间不敏感的场景。  
AWS CloudFront 是内容分发网络，不用于数据存储。  
EBS-backed storage 是块存储，适合频繁访问，成本较高。  
S3 Reduced Redundancy Storage (RRS) 提供较低的冗余但访问速度快，成本也高于 Glacier，不适合极低成本和延迟要求的归档。  
  
6. Which of the following is NOT a disaster recovery option in the cloud?
    - A. Multi-Site    
    - B. Warm standby
    - C. Single Site   
    - D. Pilot light

    <details markdown=1><summary markdown='span'>Answer</summary>  
      Correct answer: C      
    </details>

7. Which of the following services helps provide a connection from on-premises infrastructure to resources hosted in the AWS Cloud. (Select 2)  !
    - A. AWS Subnets   
    - B. AWS VPC
    - C. AWS Direct Connect 
    - D. AWS VPN

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:   CD
    </details>

8. Which of the following is a best practice when working with permissions in AWS?
    - A. Ensure the highest privilege access is used     
    - B. Don’t use IAM users and groups  
    - C. Ensure the least privilege access is used   
    - D. Use the root account credentials

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  C   
    </details>  

9. What is the concept of an AWS region?
    - A. It is the same as an Availability zone     
    - B. It is a collection of Compute capacity  
    - C. It is a geographical area divided into Availability Zones  
    - D. It is a collection of Edge locations

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  C   
    </details>  

10. What acts as a firewall that controls the traffic allowed to reach one or more instances? !
    - A. EC2     
    - B. IAM
    - C. Security group     
    - D. ACL    

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  C   
    </details>

Security Group 是一种虚拟防火墙，控制进入和离开一个或多个EC2实例的网络流量。它基于允许的规则来过滤流量。  
ACL（Network Access Control List） 也用于控制子网级别的流量，但它作用在子网层面，而不是直接作用于实例。  
EC2 是实例本身，不是防火墙。  
IAM（Identity and Access Management） 管理身份和权限，不负责网络流量控制。  
  
11. In your AWS Organization, there are two accounts: one for Development (Dev) and another for Quality Assurance (QA). Both are part of a consolidated billing system managed by the master account. The master account has purchased three Reserved Instances, a billing model offering discounted rates compared to On-Demand pricing.  Currently, the Dev team is utilizing two of these Reserved Instances. The QA team plans to deploy three instances. How will the instances used by the QA team be billed according to the available pricing models? !
    - A. Three Reserved and no On-Demand
    - B. Two Reserved and one On-Demand
    - C. No Reserved and three On-Demand   
    - D. One Reserved and two On-Demand  

    <details markdown=1><summary markdown='span'>Answer</summary>  
      Correct answer: D  
    </details>

12. You are exploring what services AWS has off-hand. You have a large number of data sets that need to be processed. Which of the following services can help fulfil this requirement. !
    - A. Storage gateway   
    - B. Glacier
    - C. EMR     
    - D. S3

    <details markdown=1><summary markdown='span'>Answer</summary>  
      Correct answer:  C   
    </details>

EMR 是托管的大数据处理服务，支持 Hadoop、Spark 等框架，专门用于批量处理和分析大规模数据集。  
Storage Gateway 是混合云存储服务，主要用于**连接本地存储和云存储**，**不用于数据处理**。  
Glacier 是长期归档存储，主要用于冷数据存储，不适合频繁处理。  
S3 是对象存储，适合存储大量数据，但本身**不处理数据**。  
  
13. When working on the costing for on-demand EC2 instances, which of the following attributes determine the cost of the EC2 Instance? (Select 3) !
    - A. Edge location   
    - B. Instance Type
    - C. Location Type       
    - D. AMI Type

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  BCD 
    </details>
  
Instance Type（实例类型）决定CPU、内存等资源配置，影响价格。  
Location Type 指的是所在区域（Region），不同区域价格不同。  
AMI Type（Amazon Machine Image类型）会影响价格，尤其是带有商业软件许可的AMI会更贵。  
Edge location 主要用于**内容分发网络**（CloudFront），**不影响EC2实例定价**。  
  
14. What does Amazon EC2 provide?  !
    - A. Physical servers, remotely managed by the customer.    
    - B. Computer Clusters in the Cloud.
    - C. Virtual servers in the Cloud.   
    - D. A platform to run code (Java, PHP, Python), paying on an hourly basis.

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  C   
    </details>
mazon EC2 本身不直接提供集群，而是提供构建集群所需的虚拟服务器基础设施。  
  
15. Which of the following AWS services automatically increases or decreases the number of resources (such as EC2 or ECS) running in a group based on demand? !
    - A. AWS Inspector      
    - B. AWS Auto Scaling
    - C. AWS ELB   
    - D. AWS EC2

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer: B  
    </details>

AWS Inspector用于**安全漏洞扫描**，不是用来扩缩资源的。  
AWS ELB（Elastic Load Balancing）用于将**流量分发**到多个实例，自己不自动调整实例数量。  
AWS EC2 是虚拟服务器服务，**不具备自动扩缩功能**，需要搭配 Auto Scaling 来实现动态调整。  
  
16. Which of the following is AWS services allows you to build a data warehouse on the cloud? !
    - A. AWS EMR   
    - B. AWS Storage Gateway
    - C. AWS Snowball     
    - D. AWS Redshift

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  D   
    </details>

AWS EMR（Elastic MapReduce）**用于大数据处理**（如 Hadoop、Spark），不是数据仓库，适合复杂的数据转换和处理。  
AWS Storage Gateway 是**连接本地存储和 AWS 云存储**的服务，不用于数据仓库。  
AWS Snowball是一种**物理设备**，用于**大规模数据迁移**到云中，不用于构建数据仓库。  
  
17.  How do you backup an EBS Volume? !     
    - A. Store Backups in Glacier     
    - B. EBS Automatic Backups
    - C. EBS Snapshot 
    - D. Store Backups in S3

    <details markdown=1><summary markdown='span'>Answer</summary>  
      Correct answer:   C
    </details>

Store Backups in Glacier：是用于长期归档的冷存储，不能直接用于备份 EBS 卷。  
EBS Automatic Backups： **没有名为 "EBS Automatic Backups" 的具体服务**，自动快照需要手动配置或使用 AWS Backup。  
Store Backups in S3： 虽然EBS快照确实存储在 S3 中，但这个过程是由 AWS 管理的，你不能手动将 EBS 备份直接存入 S3。  
  
18.  You have a distributed application that regularly processes large amounts of data across multiple Amazon EC2 instances and can recover smoothly from interruptions. This application does not require continuous, dedicated compute capacity. What is the most cost-effective way to ensure the availability of this application?     
    - A. On-Demand instances   
    - B. Dedicated instances  
    - C. Spot Instances     
    - D. Reserved instances

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:  C   
    </details>

On-Demand instances：按需实例，灵活但价格高，不适合节省大量成本的场景。  
Dedicated instances：提供物理隔离，价格最贵，适合有合规或物理隔离要求的场景。  
Reserved instances ：适用于持续运行的长期负载，但如果应用运行是间歇性的，会浪费资源。  
  
19. Which of the following IAM identities allow an application deployed on an EC2 instance to write data to S3 in a secure manner?  !
    - A. AWS IAM Permissions     
    - B. AWS IAM Groups
    - C. AWS IAM Roles   
    - D. AWS IAM Users  

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:   C
    </details>

20. AWS provides a storage option known as Amazon S3 Glacier. What is this AWS service designed for? (Select 2)  !
    - A. Active database storage   
    - B. Cached session data
    - C. Data archives 数据归档！
    - D. Infrequently accessed data  

    <details markdown=1><summary markdown='span'>Answer</summary>
      Correct answer:   CD  
    </details>








