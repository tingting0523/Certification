1. A company plans to use an Amazon Snowball Edge device to transfer les to the AWS Cloud. Which activities related to a Snowball Edge device are available to the company at no cost?    
    - A. Use of the Snowball Edge appliance for a 10-day period
    - B. The transfer of data out of Amazon S3 and to the Snowball Edge appliance
    - C. The transfer of data from the Snowball Edge appliance into Amazon S3  
    - D. Daily use of the Snowball Edge appliance after 10 days  

    <details markdown=1><summary markdown='span'>Answer</summary>      
      Correct answer: C 
    </details>


2.  A company has deployed applications on Amazon EC2 instances. The company needs to assess application vulnerabilities and must identify infrastructure deployments that do not meet best practices. Which AWS service can the company use to meet these requirements?      
    - AWS Trusted Advisor
    - B. Amazon Inspector
    - C. AWS Cong
    - D. Amazon GuardDuty   

    <details markdown=1><summary markdown='span'>Answer</summary>          
      Correct answer: B    
    </details>  

3. A company has a centralized group of users with large le storage requirements that have exceeded the space available on premises. The company wants to extend its le storage capabilities for this group while retaining the performance benet of sharing content locally. What is the MOST operationally ecient AWS solution for this scenario?       
    - A. Create an Amazon S3 bucket for each user. Mount each bucket by using an S3 le system mounting utility.  
    - B. Congure and deploy an AWS Storage Gateway le gateway. Connect each user’s workstation to the le gateway.
    - C. Move each user’s working environment to Amazon WorkSpaces. Set up an Amazon WorkDocs account for each user.
    - D. Deploy an Amazon EC2 instance and attach an Amazon Elastic Block Store (Amazon EBS) Provisioned IOPS volume. Share the EBS volume
directly with the users.   

    <details markdown=1><summary markdown='span'>Answer</summary>          
      Correct answer: B
    </details>

4.  According to security best practices, how should an Amazon EC2 instance be given access to an Amazon S3 bucket?  
    - A. Hard code an IAM user’s secret key and access key directly in the application, and upload the le.
    - B. Store the IAM user’s secret key and access key in a text le on the EC2 instance, read the keys, then upload the le.
    - C. Have the EC2 instance assume a role to obtain the privileges to upload the le.  
    - D. Modify the S3 bucket policy so that any service can upload to it at any time.     

    <details markdown=1><summary markdown='span'>Answer</summary>        
      Correct answer: C
    </details>



5.  Which option is a customer responsibility when using Amazon DynamoDB under the AWS Shared Responsibility Model?        
    - A. Physical security of DynamoDB
    - B. Patching of DynamoDB
    - C. Access to DynamoDB tables  
    - D. Encryption of data at rest in DynamoDB     

    <details markdown=1><summary markdown='span'>Answer</summary>          
      Correct answer: C
    </details>

6. Which option is a perspective that includes foundational capabilities of the AWS Cloud Adoption Framework (AWS CAF)?     
    - A. Sustainability  
    - B. Performance eciency  
    - C. Governance  
    - D. Reliability     

    <details markdown=1><summary markdown='span'>Answer</summary>            
      Correct answer: C  
    </details>

7. A company is running and managing its own Docker environment on Amazon EC2 instances. The company wants an alternative to help manage cluster size, scheduling, and environment maintenance. Which AWS service meets these requirements?     
    -  A. AWS Lambda
    -  B. Amazon RDS
    -  C. AWS Fargate
    -  D. Amazon Athena  

    <details markdown=1><summary markdown='span'>Answer</summary>        
      Correct answer:  C 
    </details>    


8. A company wants to run a NoSQL database on Amazon EC2 instances. Which task is the responsibility of AWS in this scenario?     
    - A. Update the guest operating system of the EC2 instances.
    - B. Maintain high availability at the database layer.  
    - C. Patch the physical infrastructure that hosts the EC2 instances.
    - D. Congure the security group rewall.         

    <details markdown=1><summary markdown='span'>Answer</summary>          
      Correct answer: C
    </details>

9. Which AWS services or tools can identify rightsizing opportunities for Amazon EC2 instances? (Choose two.)   
    - A. AWS Cost Explorer
    - B. AWS Billing Conductor
    - C. Amazon CodeGuru
    - D. Amazon SageMaker  
    - E. AWS Compute Optimizer       

    <details markdown=1><summary markdown='span'>Answer</summary>            
      Correct answer: AE  
    </details>

10. Which of the following are benets of using AWS Trusted Advisor? (Choose two.)     
    - A. Providing high-performance container orchestration
    - B. Creating and rotating encryption keys
    - C. Detecting underutilized resources to save costs
    - D. Improving security by proactively monitoring the AWS environment  
    - E. Implementing enforced tagging across AWS resources       

    <details markdown=1><summary markdown='span'>Answer</summary>        
      Correct answer: CD  
    </details>


11.  Which of the following is an advantage that users experience when they move on-premises workloads to the AWS Cloud?    
    - A. Elimination of expenses for running and maintaining data centers      
    - B. Price discounts that are identical to discounts from hardware providers
    - C. Distribution of all operational controls to AWS  
    - D. Elimination of operational expenses       

    <details markdown=1><summary markdown='span'>Answer</summary>                  
      Correct answer: A    
    </details>

12.  A company wants to manage deployed IT services and govern its infrastructure as code (IaC) templates. Which AWS service will meet this requirement?    
    - A. AWS Resource Explorer
    - B. AWS Service Catalog        
    - C. AWS Organizations
    - D. AWS Systems Manager       

    <details markdown=1><summary markdown='span'>Answer</summary>            
      Correct answer: B(待确认)
    </details>

13. Which AWS service or tool helps users visualize, understand, and manage spending and usage over time?     
    - A. AWS Organizations
    - B. AWS Pricing Calculator
    - C. AWS Cost Explorer
    - D. AWS Service Catalog           

    <details markdown=1><summary markdown='span'>Answer</summary>          
      Correct answer:  C 
    </details>


14. A company is using a central data platform to manage multiple types of data for its customers. The company wants to use AWS services to discover, transform, and visualize the data. Which combination of AWS services should the company use to meet these requirements? (Choose two.)     
    - A. AWS Glue
    - B. Amazon Elastic File System (Amazon EFS)
    - C. Amazon Redshift
    - D. Amazon QuickSight
    - E. Amazon Quantum Ledger Database (Amazon QLDB)     

    <details markdown=1><summary markdown='span'>Answer</summary>        
      Correct answer: AD
    </details>

15.  A global company wants to migrate its third-party applications to the AWS Cloud. The company wants help from a global team of experts to complete the migration faster and more reliably in accordance with AWS internal best practices. Which AWS service or resource will meet these requirements?      
    - A. AWS Support  
    - B. AWS Professional Services      
    - C. AWS Launch Wizard  
    - D. AWS Managed Services (AMS)   

    <details markdown=1><summary markdown='span'>Answer</summary>            
      Correct answer: B
    </details>

16.  An e-learning platform needs to run an application for 2 months each year. The application will be deployed on Amazon EC2 instances. Any application downtime during those 2 months must be avoided. Which EC2 purchasing option will meet these requirements MOST cost-effectively?      
    - A. Reserved Instances  
    - B. Dedicated Hosts    
    - C. Spot Instances  
    - D. On-Demand Instances     

    <details markdown=1><summary markdown='span'>Answer</summary>        
      Correct answer: D(?)  
    </details>


17.  A developer wants to deploy an application quickly on AWS without manually creating the required resources. Which AWS service will meet these requirements?      
    - A. Amazon EC2  
    - B. AWS Elastic Beanstalk  
    - C. AWS CodeBuild          
    - D. Amazon Personalize         

    <details markdown=1><summary markdown='span'>Answer</summary>        
      Correct answer: B
    </details>

18. A company is storing sensitive customer data in an Amazon S3 bucket. The company wants to protect the data from accidental deletion or overwriting. Which S3 feature should the company use to meet these requirements?     
    - A. S3 Lifecycle rules      
    - B. S3 Versioning  
    - C. S3 bucket policies
    - D. S3 server-side encryption   

    <details markdown=1><summary markdown='span'>Answer</summary>            
      Correct answer: B    
    </details>  

19. Which AWS service provides the ability to manage infrastructure as code?
    - A. AWS CodePipeline    
    - B. AWS CodeDeploy
    - C. AWS Direct Connect
    - D. AWS CloudFormation           

    <details markdown=1><summary markdown='span'>Answer</summary>          
      Correct answer: D  
    </details>


20. An online gaming company needs to choose a purchasing option to run its Amazon EC2 instances for 1 year. The web trac is consistent, and any increases in trac are predictable. The EC2 instances must be online and available without any disruption. Which EC2 instance purchasing option will meet these requirements MOST cost-effectively?      
    - A. On-Demand Instances
    - B. Reserved Instances      
    - C. Spot Instances
    - D. Spot Fleet      

    <details markdown=1><summary markdown='span'>Answer</summary>            
      Correct answer: B
    </details>  

2.    
    -    

    <details markdown=1><summary markdown='span'>Answer</summary>          
      Correct answer: 
    </details>

2.    
    -    

    <details markdown=1><summary markdown='span'>Answer</summary>        
      Correct answer: 
    </details>

