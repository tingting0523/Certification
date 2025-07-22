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

AWS Lambda 是一种无服务器（serverless）计算服务，允许你运行代码而无需管理服务器。你只需上传代码，Lambda 会自动处理计算资源的分配、扩展和维护。

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
**AWS S3 Reduced Redundancy Storage**：Amazon S3 早期提供的一种低成本存储选项，它将对象的副本数量减少，从而降低存储成本，适用于容错要求不高的非关键数据。 

**EBS**  
Elastic Block Store 持久化的块存储服务，专门为 EC2 实例设计，用于存储数据卷（类似硬盘）  
块存储 Block Storage  
1. **Amazon EBS Snapshots** 是某个时间点上 EBS 卷数据的**增量备份**，存储在 Amazon S3 中  
2. **Amazon EBS Volumes** 具体**存储单元**，相当于云硬盘  

**Glacier**  
AWS 提供的超低成本云存储服务，专为长期归档和**不频繁访问的数据**设计。  
放很久都不怎么用的数据  
是 Amazon S3 的归档层，与 S3 无缝集成  

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


**Snowball**  
**大规模数据迁移**的物理设备服务，适用于无法通过网络快速传输数据到云端的场景  
用于数据中心迁移、灾难恢复、无法联网地区、大数据处理  
快速、离线、安全，适用于10TB–1PB 数据迁移  



**Glue、Redshift、QuickSight**   
原始数据   
--（Glue自动采集清洗转换）--〉AWS GLUE ETL  
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





**Amazon DynamoDB**
托管的 **NoSQ数据库服务**，具备亚毫秒级延迟、高可用性和自动扩展能力，适用于大规模应用和实时工作负载。  
适合存储结构化或半结构化的数据  

**Amazon RDS**  
Relational Database Service 关系型数据库服务


**Amazon ElastiCache**  
内存缓存服务，支持 Redis 和 Memcached，用于**加速 Web 应用和数据库性能**。  


**CloudFront/CDN**  
**内容分发**网络（CDN）服务，用于将网页、视频、图片和其他静态/动态内容快速、安全地分发给全球用户。  
“中转仓库”，在全球各地放置内容副本（缓存），让用户就近获取资源，提升访问速度，降低延迟和源站压力。  
mainly also for caching 


**AWS VPC**  
Virtual Private Cloud 虚拟私有云：私有网络环境  


**AWS VPN**  
网络连接服务   
连接本地网络与VPC的安全桥梁，保证跨网络数据加密传输  

**Edge Locations**  
分布在全球的边缘数据中心，用于**缓存最常访问**的内容（热门文件，eg. web pages, images and videos）。目的：缩短内容从服务器到最终用户的传输距离。  

**Regional Edge Caches / Locations**  
位于靠近边缘站点的大型缓存中心，**缓存不太热门**但仍有访问需求的内容。目的：减少回源请求次数，降低传输成本，提高性能。


**Instance Type、Location Type、AMI Type**  
1. **Instance Type**：**EC2实例的硬件规格**，决定计算资源（CPU、内存、存储、网络性能）的规格和价格。适用于选择适合**应用性能需求和成本预算**的实例。  
2. **Location Type**：**资源的地理/物理位置类型**。类型包含Region、Availability Zone、Edge Location、Wavelength Zone。适用于决定**资源的延迟、合规和灾备策略**。  
3. **AMI Type**：Amazon Machine Image，用来**启动 EC2 实例的系统镜像类型**。适用于**快速启动预配置环境的实例**。  


**AWS Inspector监察员**  
“云安全体检师”，自动扫描并给出详细的安全报告和修复建议  

**instances types**  
1. **On-Demand instances**：物理隔离，灵活但**价格最高**
2. **Dedicated instances**：物理隔离，能更细粒度管理服务器资源，**价格高**
3. **Spot Instances**：适合弹性强、能容忍中断的任务，因为实例会被 AWS 回收（提前两分钟通知）利用 AWS 闲置容量，**价格最低**
4. **Reserved instances**：适合长期、稳定使用，**价格较低但仍比 Spot 高**
   
Security group



**Serverless**  
serverless means you do not need to worry about the data or the code, you just need to plug in. 你不需要管理服务器基础设施(服务器的启动、配置、运维、扩缩容)
Lambda、ECS Fargate、function as a service





