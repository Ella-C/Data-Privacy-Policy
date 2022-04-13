# Data Privacy Policy

Our Privacy Policy was last updated on 2022-02-25.

This Privacy Policy describes how we collect,use,process,dispose,and store the data from AWS. Our primary data center would take AWS Data Lake solution.


## Definitions

- Amazon S3 : Amazon Simple Storage Service 
- Amazon S3 Glacier : mazon Simple Storage Service Glacier 
- Data Lake : An architectural approach that allows us to store all our data in a centralized repository, so that it can be categorized, catalogued, secured, and analyzed by a diverse set of users and tools.
- AWS KMS : Amazon Web Service Key Manager Service.
- PII : Personally Identifiable Information.


## Access policy

-  Define a bucket policy to manage permissions for cross-account access, and manage permissions for users in another account. Bucket policies can be defined based on various factors, such as S3 operations, type of requestor, type of resources, and the nature of the request. A bucket policy defined for a bucket is applicable for all the objects in the bucket. This way we can manage the permissions for all the objects centrally instead of managing access for individual objects. 
-  Use access-control lists to manage permissions to a bucket or an object.Access-control lists can only provide read/write permissions to an object or bucket and grant bucket permission to other accounts or users in other accounts. 
-  Use user policies so that permissions to access data assets can also be linked to user roles and permissions for the data processing and analytics services and tools that our data lake users will use.


## Data encryption with Amazon S3 and AWS KMS

- Use AWS KMS to scale and simplify management of encryption keys. AWS KMS gives us centralized control over the encryption keys used to protect our data assets. We can create, import, rotate, disable, delete, define usage policies for, and audit the use of encryption keys used to encrypt our data. 
- For PII data, use AWS CloudHSM to store the keys authorize AWS KMS to use it as a dedicated key store.


## Protecting data with Amazon S3

- Data protection rests on the inherent durability of the storage platform used.The durability of Amazon S3 is designed so that 10,000,000 data assets can be reliably stored for 10,000 years.
- S3 provides versioning to protect data assets against unintentional and malicious deletion and corruption,whether through users accidentally deleting data assets, applications inadvertently deleting or corrupting data, or rogue actors trying to tamper with the data. 
- S3 Cross-Region Replication is an integral S3 capability that automatically and asynchronously copies data assets from a data lake in one AWS Region to a data lake in a different AWS Region. The data assets in the second Region are exact replicas of the source data assets that they were copied from, including their names, metadata, versions, and access controls. All data assets are encrypted during transit with SSL to ensure the highest levels of data security.
- S3 Object Lock allows us to write objects using the WORM model. We can use Object Lock for scenarios which make it imperative that the data is not updated or deleted after it is written. 


---
END OF POLICY


