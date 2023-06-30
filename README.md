# web-app-cloudformation-stack
Deploy a Wordpress application using  AWS CloudFormation templates 
AWS Wellarchitectedlabs
https://www.wellarchitectedlabs.com/security/200_labs/200_automated_deployment_of_ec2_web_application/
https://www.wellarchitectedlabs.com/security/200_labs/200_automated_deployment_of_vpc/

1. Create a VPC stack
•	VPC
•	Public and Private Subnets
•	Route Tables
•	NAT gateway
•	Internet gateway
2. Create a Web Stack
•	Application load balancer
•	Auto scaling group of web instances
•	A role attached to the auto-scaled instances allows temporary security credentials to be used
•	Instances use Systems Manager instead of SSH for administration
•	Amazon Aurora serverless database cluster
•	Secrets manager secret for database cluster
•	AWS Key Management Service is used for key management of Aurora database
•	Security groups for load balancer and web instances to restrict network traffic
•	Custom CloudWatch metrics and logs for web instances
•	IAM role for web instances that grants permission to Systems Manager and CloudWatch
•	Instances are configured from the latest Amazon Linux 2 Amazon Machine Image at boot time using user data to install agents and configure services


