**SNS**  
SNS 发布消息 → SQS 订阅接收
**SQS（Simple Queue Service）** 
托管的消息队列服务。  
解耦系统、提升弹性和稳定性的关键组件，支持高并发、灵活可靠的异步消息通信。  
例如：前端把请求信息发送到一个“队列”（SQS）中，后端从队列中一个一个地取出请求来处理。  

**Lambda、EC2**  
EC2 / Lambda：消费 SQS 中的消息，触发后台处理  
1.Lambda：Serverless Function 服务，让你只需上传代码即可运行，不需管理任何服务器。  
2.EC2（Elastic Compute Cloud）：弹性云服务器服务，允许你像管理传统主机一样运行虚拟机--全功能云服务器  

**IAM**  
IAM：Identity and Access Management AWS 提供的身份与权限管理服务，允许你安全地控制用户和资源之间的访问权限。  
1. AWS IAM Permissions：  
2. AWS IAM Groups：用户集合，可统一分配权限策略  
3. AWS IAM Roles：可临时扮演的身份，常用于跨账户、服务访问（比如 EC2 访问 S3）  
4. AWS IAM Users：单个身份，对应一个人或应用程序，拥有一组凭证（密码/访问密钥）  

**ACL**  
Access Control List，访问控制列表

S3
EMR
ELB
AMI
AWS Snowball
AWS Redshift
Storage gateway
Amazon EBS Snapshots
Amazon EBS Volumes
Amazon Glacier
Amazon DynamoDB
Amazon RDS
Amazon ElastiCache
Amazon Simple Object Storage
AWS CloudFront
AWS S3 Reduced Redundancy Storage
AWS Subnets
AWS VPC
AWS Direct Connect
AWS VPN
Edge location
Instance Type、Location Type、AMI Type
AWS Inspector监察员
On-Demand instances、Dedicated instances、Spot Instances、Reserved instances
Security group




