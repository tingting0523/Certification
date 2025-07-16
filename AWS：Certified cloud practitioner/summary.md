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


**S3**  
Simple Storage Service  AWS提供的可扩展、高可用、安全的对象存储服务  
无限容量的网盘/硬盘，但是放在云端；你可以把文件（叫“对象”）上传到云端，分类保存在文件夹（叫“桶” bucket）里。 
对象存储 Object Storage   

**EBS**  
Elastic Block Store 持久化的块存储服务，专门为 EC2 实例设计，用于存储数据卷（类似硬盘）  
块存储 Block Storage  
1. **Amazon EBS Snapshots** 是某个时间点上 EBS 卷数据的**增量备份**，存储在 Amazon S3 中  
2. **Amazon EBS Volumes** 具体**存储单元**，相当于云硬盘  

**Storage gateway**  
混合**云存储服务**，**连接本地环境与AWS云存储**，实现数据的无缝迁移、备份和归档 

**Storage gateway、EBS、Storage gateway**  
1. EBS：云上的“硬盘”，给单台服务器（EC2）当系统盘或数据盘用，适合需要快速随机访问的场景。   
2. Storage Gateway：是“桥梁”和“同步工具”，让你本地数据和云端存储无缝协作，实现备份、归档和混合云存储。  
3. S3：是“海量文件仓库”，存放各种静态数据，像图片、视频、备份文件等，面向互联网和大规模数据访问。  

**EMR**  
Elastic MapReduce 托管大数据处理服务，可以用来运行 Apache Spark、Hadoop、Flink、Hive、Presto 等框架，用于大规模数据分析、机器学习、ETL 处理等任务  
用于处理 TB / PB 级别的大数据，帮助你在 AWS 上搭建一个弹性伸缩的大数据集群，不必自己维护底层服务器和软件环境。  


**ELB**  
Elastic Load Balancer 自动分发流量到多个目标（如 EC2 实例、容器、IP 地址等）的**负载均衡服务**，用于实现高可用性、故障转移与弹性扩展。


**AMI**  
Amazon Machine Image 启动EC2实例的模板镜像，包含了操作系统、预装软件、配置文件等内容，是 EC2 的“操作系统快照”  
可以用它快速创建、复制、恢复和部署服务器环境  
一份 AMI 可以启动多个 EC2，像“批量复制系统”  


**Snowball**。
**大规模数据迁移**的物理设备服务，适用于无法通过网络快速传输数据到云端的场景  
用于数据中心迁移、灾难恢复、无法联网地区、大数据处理  
快速、离线、安全，适用于10TB–1PB 数据迁移  



**Glue、Redshift、QuickSight**   
原始数据 --（Glue自动采集清洗转换）--〉AWS GLUE ETL  
        -- (数据加载)--〉Amazon Redshift数据仓库  
        --（查询分析）--〉Amazon QuickSight可视化和BI  

1. **AWS Glue**  
serverless的托管数据集成服务，用于**自动发现、准备和转换数据**，方便在数据湖、数据仓库和数据库间进行ETL处理。  
数据的“万能搬运工”和“清洗师”,自动生成 ETL 代码，帮你转换、清洗、准备数据  
2. **Redshift**  
高速、完全托管的**云数据仓库服务**，用于大规模数据分析和复杂查询  
列式存储，支持标准 SQL 查询，兼容多种 BI 工具（如 Tableau、Power BI）  
能够快速处理数 TB 到 PB 级别的数据  
3. **Amazon QuickSight**
AWS提供的快速、云端托管的商业智能（BI）服务，用于创建交互式数据可视化和仪表盘。  
QuickSight 是一款**在线工具**，帮助用户轻松连接数据源，**快速生成图表、报表和仪表盘**  


**EFS**  
Elastic File System 弹性、可扩展的网络文件系统，允许多个 EC2 实例同时挂载访问共享文件存储  
就像一个“云端的共享硬盘”  

**Amazon QLDB**  
Amazon Quantum Ledger Database 完全托管的分类账数据库，提供透明、不可篡改和可验证的交易日志，适合记录关键业务数据的变化历史  
它会自动记录所有数据变更，并保存一份**不可修改**且可验证的历史记录  



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




