---
title : "Week 7 Worklog"
date :  "`r Sys.Date()`" 
weight : 7
chapter : false
pre : "<b>1.7. </b>"
---
### Week 7 Objectives
* Integrate Amazon S3 into the web application for file storage. 
* Replace local file storage with cloud-based storage. 
* Understand S3 permissions, bucket policies, and access control. 
* Improve system scalability and storage efficiency. 

### Tasks to be carried out this week
|Day|Task|Start Date|Completion Date|Reference Material
|:-:|---|:-:|:-:|:-:|
|2|<ul style="margin:0"><li>Create S3 bucket with appropriate naming convention</li><li>Configure region and storage settings</li><li>Disable block public access (for testing)</li></ul>|20/04/2026|20/04/2026|AWS Console|
|3|<ul style="margin:0"><li>Configure bucket policy and IAM permissions</li><li>Allow public read access for images</li><li>Test access via S3 URL</li></ul>|21/04/2026|21/04/2026|[AWS Docs](https://cloudjourney.awsstudygroup.com/)|
|4|<ul style="margin:0"><li>Integrate S3 into PHP application</li><li>Install AWS SDK for PHP</li><li>Configure credentials and region</li></ul>|22/04/2026|22/04/2026|AWS SDK Docs|
|5|<ul style="margin:0"><li>Implement file upload to S3</li><li>Retrieve and store S3 file URL in database</li><li>Modify application logic to use S3 URLs</li></ul>|23/04/2026|23/04/2026|PHP Docs|
|6|<ul style="margin:0"><li>Test file upload, display, and deletion</li><li>Debug upload errors (permission, size limit)</li><li>Optimize file handling performance</li></ul>|24/04/2026|24/04/2026||

### Acheievements
* Successfully created and configured an Amazon S3 bucket for storing application files. 
* Configured access control and permissions: 
  * Applied bucket policy to allow public read access for static files
  * Managed IAM permissions for secure access
  * Understood security implications of public access
* Integrated S3 into the web application: 
  * Installed and configured AWS SDK for PHP
  * Connected application to S3 using credentials and region settings
* Implemented file upload functionality: 
  * Uploaded files directly from application to S3
  * Generated and retrieved S3 object URLs
  * Stored file URLs in database instead of local paths
* Modified application logic: 
  * Replaced local file handling with cloud-based storage
  * Ensured images and files are loaded from S3 URLs
* Tested full file workflow: 
  * Upload file → Store URL → Display image
  * Verified file accessibility via public URL
* Identified and resolved common issues: 
  * Permission errors due to incorrect bucket policy
  * File upload size limitations
  * Incorrect MIME type handling
* Improved system architecture: 
  * Separated storage layer (S3) from compute (EC2)
  * Increased scalability and flexibility
  * Reduced dependency on server local storage