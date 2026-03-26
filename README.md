# Architecture
terraform-project/
├── main.tf
├── variables.tf
├── terraform.tfvars
├── outputs.tf         
│
├── modules/
│   ├── vpc/
│   │   ├── main.tf
│   │   ├── variables.tf
│   │   ├── outputs.tf   
│   │
│   ├── ec2/
│   │   ├── main.tf
│   │   ├── variables.tf
│   │   ├── outputs.tf   
│   │
│   ├── s3/
│       ├── main.tf
│       ├── variables.tf
│       ├── outputs.tf  


1. create resource for VPC, EC2 and S3 in respective main.tf files in modules
2. create variables for VPC, EC2 and S3 in respective variables.tf files in modules
3. create outputs for VPC, EC2 and S3 in respective outputs.tf files in modules
4. call the modules in main.tf and pass the variables   
5. create terraform.tfvars file and assign values to variables
6. run terraform init, plan and apply to create the infrastructure
7. verify the created resources in AWS console
8. run terraform destroy to clean up the resources after verification


