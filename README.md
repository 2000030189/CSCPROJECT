# VOTING APPLICATIONS USING AWS SERVICES
![image](https://user-images.githubusercontent.com/96165337/231077922-7f16c5e3-8fea-4ccf-adba-9d8ae5be60c0.png)
# Steps to Build the Architecture:
  
Step1:Create Table in Amazon DynamoDB.

Step2: Create a Lambda Function (NodeJS)

Step3:Create a new role

Step 4:After creation of this role attach some more policies

Go to lambda function
Write the code and deploy it and test the event

Step-5:Create a Another Lambda Function integrate with Dynamo DB(ADD Trigger)
Add the code CastVoteJSON

Step 6:API Gateway.Configure API gateway

Step 7:Create the above Resource->create a method POST

Step 8:Create post method Add Lambda Function to it and add mapping template code.

Step 9:In Method response remove 200 and ADD 204

Step 10: In Integration response Add 204 in default and remove 200.

Step-11:Click on Test

Step 12: Copy Invoke URL and add it in index.html

Create an S3 bucket with the static web hosting
Upload the files in S3.

Step 13:Add s3 files in bucket with default settings add bucket policy and enable static Website HostingAdd Bucket Policy

Step 14: Go to S3 Bucket Properties -> static hosting ->Copy Url
