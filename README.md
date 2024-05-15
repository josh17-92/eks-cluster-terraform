# terraform-eks
I'm using modules to create an EKS cluster on AWS using Terraform.

### Install AWS CLI 

As the first step, you need to install AWS CLI as we will use the AWS CLI (`aws configure`) command to connect Terraform with AWS in the next steps.

Follow the below link to Install AWS CLI.
```
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
```

### Install Terraform

Next, Install Terraform using the below link.
```
https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli
```

### Connect Terraform with AWS

It's very easy to connect Terraform with AWS. Run `aws configure` command and provide the AWS Security credentials (I recommend storing your credentials on a Vault)

### Initialize Terraform

Clone the repository and Run `terraform init`. This will initialize the terraform environment and download the required modules, providers, and other configurations.

### Optionally review the terraform configuration

Run `terraform plan` to see the configuration it creates when executed.

### Finally, Apply terraform configuration to create an EKS cluster with VPC 

Run `terraform apply` and Terraform will start configuring your services on AWS

### NOTE

Always go through the Terraform documentation, as some modules might be updated and some arguments could be unsupported or deprecated
