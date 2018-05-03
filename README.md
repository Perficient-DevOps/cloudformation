## CloudFormation templates
Various CloudFormation templates for doing this and that.

### DevOps-in-a-Box
A set of templates in `doiab` to stand-up an integrated toolchain (WIP). Must be run sequentially:
* **iam.json** creates a managed policy, role, and instance profile for EC2 instances
* **vpc.json** creates a VPC with 2 private and 2 public subnets, a NAT Gateway, VPC Endpoints for S3 and Dynamo, and preconfigured route tables
* **security-groups.json** creates a set of security groups for Jenkins, Nexus, and the UrbanCode products
* **server-nodes.json** creates EC2 instances using based on IAM and security groups

### Atlassian
Modified versions of the Atlassian Quick Start offerings in `atlassian`:
* [Bitbucket Data Center](https://aws.amazon.com/quickstart/architecture/bitbucket/) - Modified to allow for smaller EC2/RDS/Elasticsearch types
* [Jira Data Center](https://aws.amazon.com/quickstart/architecture/jira/) - Modified to allow for smaller EC2/RDS instance types and to use ALB

### AWS
Templates from AWS in `aws`:
* [VPC with dedicated NACLs for each private subnet](https://github.com/aws-quickstart/quickstart-aws-vpc)