## Learning Terraform 
Learn Backend and Variables

## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 5.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | ~> 5.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_dynamodb_table.basic-dynamodb-table](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/dynamodb_table) | resource |
| [aws_instance.my_first_instance](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |
| [aws_kms_alias.a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kms_alias) | resource |
| [aws_kms_key.a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kms_key) | resource |
| [aws_s3_bucket.example](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [aws_s3_bucket_versioning.versioning_example](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_versioning) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_ami"></a> [ami](#input\_ami) | this is the machine image which is region specific | `string` | `"ami-080e1f13689e07408"` | no |
| <a name="input_bucket_name"></a> [bucket\_name](#input\_bucket\_name) | name of my s3 bucket | `string` | `"this-is-my-bucket-plz"` | no |
| <a name="input_delete_protect"></a> [delete\_protect](#input\_delete\_protect) | To protect the dynamodb from being deleted by default | `bool` | `true` | no |
| <a name="input_deletion_window"></a> [deletion\_window](#input\_deletion\_window) | when the kms key is deleted, it will take 7-30 days number of days before it deletes totally | `number` | `30` | no |
| <a name="input_env"></a> [env](#input\_env) | tag environment name for my s3 bucket | `string` | `"Dev"` | no |
| <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type) | this is the instance type needed for my ec2 | `string` | `"t2.micro"` | no |
| <a name="input_name"></a> [name](#input\_name) | name of my ec2 | `string` | `"evans-sam"` | no |
| <a name="input_region"></a> [region](#input\_region) | This is the region where AWS resources will be deployed | `string` | `"us-east-1"` | no |
| <a name="input_role_name"></a> [role\_name](#input\_role\_name) | My iam role name | `string` | `"terraform-state-file-role"` | no |
| <a name="input_table_name"></a> [table\_name](#input\_table\_name) | Name of my dynamodb table | `string` | `"tf-state-lock-with-dynamodb"` | no |
| <a name="input_tag_name"></a> [tag\_name](#input\_tag\_name) | tag name for my s3 bucket | `string` | `"secured"` | no |
| <a name="input_team"></a> [team](#input\_team) | tag team who will be using my s3 bucket | `string` | `"cyber-security"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_ec2_public_ip"></a> [ec2\_public\_ip](#output\_ec2\_public\_ip) | n/a |
