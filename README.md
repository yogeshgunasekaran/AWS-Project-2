# AWS-Project-2
This project is to deploy a web-application in AWS cloud infrastructure using AWS Elastic Beanstalk (PaaS), Route53 Public DNS, ACM, S3, ELB, Autoscaling Group, RDS, Elastic Cache, Active MQ, CloudWatch and CloudFront 
### Project Architecture
![2](https://user-images.githubusercontent.com/106590073/180609886-65630a06-5809-47f6-ab26-dba588dee2c4.jpg)


### Procedure : 
- Login to AWS Account
- Create Key pair for beanstalk instance login
- Create Security Group for Elastic Cache, RDS and Active MQ
- Create
  - RDS
  - Amazon Elastic Cache
  - Amazon Active MQ
- Create Elastic Beanstalk Environment
- Update Security Group of backend to allow traffic from Beanstalk Security Group
- Update Security Group of backend to allow internal traffic
- Launch EC2 Instance for DB Initializing 
- Login to the instance and Initialize RDS DB
- Change healthcheck on Beanstalk to "/login"
- Add 443 HTTPS listner to ELB
- Build artifact with backend endpoints information 
- Deploy artifact to Beanstalk
- Create CDN with SSL certificate
- Update entry in GoDaddy DNS Zones
- Test the URL
- 
