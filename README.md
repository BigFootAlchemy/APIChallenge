# BigFootAlchemy's Labs
API Challenge for AWS and Python SDK

##Prerequisite : 
Install aws cli - pip install awscli
Install boto3 - pip install boto3
Sign up for free aws dev account - https://aws.amazon.com/s/dm/optimization/server-side-test/free-tier/free_np/

#API Challenges

##API Challenge Challenge Group A - Basics

Challenge 1 (5 Points) : Write a script that builds three 512 MB EC2 Instances that following a similar naming convention. (ie., web1, web2, web3) and returns the IP of each instance. Use any image you want. 

Challenge 2 (10 Points) : Write a script that snapshots a volume and creates an AMI  (takes an image and deploys the image as a new server with automation). 

Challenge 3 (5 Points) : Write a script that accepts a directory as an argument as well as a  S3 bucket name. The script should upload the contents of the specified directory to the S3 Bucket (or create it if it doesn't exist). The script should handle errors appropriately. (Check for invalid paths, etc.) 

Challenge 4 (3 Points) : Write a script that uses Route 53 to create a new A record when passed a FQDN and IP address as arguments. 

Challenge 5  (5 Points) : Write a script that creates a new DynamoDB database. Should contain at least one database, and the database should have at least one user that can connect to it. 

##API Challenge Group B - Advanced Scripting

Challenge 6 (5 Points) : Write a script that creates a public S3 website bucket. Must have the following: 
 * index file
 * error file 
 * return the status code of a curl test. 

Challenge 7 (5 Points) : Write a script that will create 2 EC2 instances and add them as nodes to a new Elastic Load Balancer. 

Challenge 8 (15 Points) : Write an application that will:
Create a new Autoscaling Group. Create a Elastic Load Balancer . Add the new ASG to the ELB .Set up ELB monitor and custom error page. Create a Route53 DNS record based on a FQDN for the ELB . Write the error page html to a file in S3 for backup failover. The Launchconfig for the ASG needs the following :   
* a valid Key Pair
* an AMI from Challenge 2 
* installs ssm
* installs CodeDeploy agent 


##API Challenge Group C - Tools

Challenge 9 (5 Points) : User Packer.io to build an AMI that when passed the arguments image and instance type it creates a new AMI with ssm, scaleft, ansible, awscli, and path. 

Challeng 10 (10 Points) : Write a python script to parse the packer json template , validate , and pass it to CodeCommit . 


##API Challenge Group D - Messaging 

Challenge 11 (1 Point) : Write an application that will create a SQS queue and send it a message. 

Challenge 12 (5 Points) : Write an application that prints hello world if the SQS queue has a message. 


##API Challenge Group E - Cleaning up
Challenge 13(10 Points) : Write a script that tags the EC2 instances with the date, creater, and a delete on date 1 week from the instance creation time . 

Challenge 14 (15 Points) : Write an application that nukes everything in you have created from these exercises. It should:
* Delete all EC2 instances
* Delete all Custom Amazon Images
* Delete all S3 Buckets
* Delete all DynamoDB
* Delete all Route53 Records
* Delete all Volumes.
