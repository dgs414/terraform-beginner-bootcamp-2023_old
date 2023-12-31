# Terraform Beginner Bootcamp 2023

## Given a version number MAJOR.MINOR.PATCH, increment the:

- **MAJOR** version when you make incompatible API changes
- **MINOR** version when you add functionality in a backward compatible manner
- **PATCH** version when you make backward compatible bug fixes

###Updating Terraform installation

[Install Terraform CLI](https://developer.hashicorp.com/terraform/downloads?ajs_aid=3db45936-e066-485e-9a0d-a1678ec8589c&product_intent=terraform)

Updated Terraform bash script

- https://www.geeksforgeeks.org/chmod-command-linux/
- https://en.wikipedia.org/wiki/Chmod

### AWS CLI Installation

https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

We can check if our AWS credentials are configured correctly by running the following command:
```
aws sts get-caller-identity
```

### Setting AWS CLI Env Vars
https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html

### Terraform Registry

https://registry.terraform.io/

- **Providers** is an interface to APIs that will allow you to create resources
- **Modules** an option to make large amounts of terraform code modular, portable and sharable.

### Terraform Main Commands

**Main commands:**
-  **`init`**          Prepare your working directory for other commands
-  **`validate`**      Check whether the configuration is valid
-  **`plan`**          Show changes required by the current configuration
-  **`apply`**         Create or update infrastructure
-  **`destroy`**       Destroy previously-created infrastructure

### AWS S3 Documentation
https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket

### AWS S3 Bucket Naming Rules

https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html?icmpid=docs_amazons3_console

```
random_string.bucket_name: Creation complete after 0s [id=GtiXuoABtL4NgMvP]
aws_s3_bucket.example: Creating...
╷
│ Error: validating S3 Bucket (GtiXuoABtL4NgMvP) name: only lowercase alphanumeric characters and hyphens allowed in "GtiXuoABtL4NgMvP"
│ 
│   with aws_s3_bucket.example,
│   on main.tf line 25, in resource "aws_s3_bucket" "example":
│   25: resource "aws_s3_bucket" "example" {
╵
```
####  Terraform Destroy
This will destroy resources
