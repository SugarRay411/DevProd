# DevProd
Web App on AWS SAAS and PAAS
ABOUT PROJECT
Multi-Tier web Application Stack (devprod)
Re-architect services for AWS Cloud
Architecture to boost agility or improve business continuity

AWS SERVICES
Beanstalk was used for VM for Tomcat server, automation for VM Scaling, Nginx Lb Replacement 
S3/EFS will be used for storage. 
RDS Instance for Databases
Elastic Cache in place of Memcache
Active MQ in place of Rabbit MQ
Route 53 for DNS
CloudFront for content delivery Network

Flow of execution Aws cloud

1. Login to AWS
2. Create key pair for beanstalk instance login
3. Create security group for Elasticcache, RDS and ActiveMQ
4. Create Elastic Beanstalk Environment
5. Update SG of backend to allow traffic from bean SG
6. Update SG of backend to allow internal traffic
7. Launch EC2 Instance for DB Initializing
8. Login to the instance and initialize RDS DB
9. Add 443 https Listener to ELB
10. Build Artifact with Backend Information
11. Deploy Artifact to Beanstalk
12. Create CDN wit ssl cert
13. Update entry in Godday DNS Zones
14. Test the URL

