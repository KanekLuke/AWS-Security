<h2>Description</h2>
<b>My Healthy Eating Inc. successfully migrated their data center to AWS cloud.<br><br></b>
Since the company’s target market is North America, they decided to deploy all resources into two availability zones, us-east-1a and us-east-1b, in the US East (N. Virginia) region. They also choose Route 53 to manage the domain names for their e-Commerce applications and AWS Certificate Manger to maintain their SSL certificates.  The e-Commerce applications have not been re-designed and are still running on top of LAMP (Linux, Apache, MySQL, and PHP) stack. Applications are deployed into two EC2 instances connecting to an EFS system for file sharing. An elastic load balancer (ELB) is in front of the EC2 instances distributing incoming traffic. Applications are also connected to a RDS MySQL instance in the database private subnet. The RDS instance has a standby instance sitting in a separate AZ. All EC2 and RDS instances are deployed in private subnets, connecting through NAT gateways to retrieve software updates from Internet. Finally, S3 is leveraged to store all the data files and a lifecycle policy is in place to move one year old data to S3 Glacier for backup.<br><br>

As a senior AWS consultant, you are recently hired by the company to help review their architecture and provide a report. In the report, you are required to address following two questions:<br>
1)	What security features need to be enabled for each of the AWS services listed? What other AWS security services should be leveraged as well to improve the security posture?<br><br>
2)	What are the top three architecture improvements that the company should make next? Use Well-Architected Framework to guide your analysis.<br>

https://drive.google.com/file/d/1H8xpcgCH7vgb2ZaP-8l-0tlObAQSgB1o/view?usp=sharing
