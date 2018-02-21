## CloudFormation templates
Various CloudFormation templates to provision AWS resources
1. **iam.json** creates a managed policy, role, and instance profile for EC2 instances
2. **vpc.json** creates a VPC with 2 private and 2 public subnets, a NAT Gateway, VPC Endpoints for S3 and Dynamo, and preconfigured route tables
3. **security-groups.json** creates a set of security groups for Jenkins, Nexus, and the UrbanCode products
4. **server-nodes.json** creates EC2 instances using based on IAM and security groups
