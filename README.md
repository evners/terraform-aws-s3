# terraform-aws-s3

This module provides a simple and efficient way to create and configure S3 buckets in your AWS environment, allowing you to easily define bucket properties, access controls, and lifecycle policies as code.

<!-- BEGIN_TF_DOCS -->

## Requirements

No requirements.

## Providers

| Name                                                      | Version |
| --------------------------------------------------------- | ------- |
| <a name="provider_aws"></a> [aws](#provider_aws)          | n/a     |
| <a name="provider_random"></a> [random](#provider_random) | n/a     |

## Modules

No modules.

## Resources

| Name                                                                                                                                                                                  | Type     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| [aws_s3_bucket.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket)                                                                           | resource |
| [aws_s3_bucket_acl.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_acl)                                                                   | resource |
| [aws_s3_bucket_ownership_controls.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_ownership_controls)                                     | resource |
| [aws_s3_bucket_policy.public_access](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_policy)                                                    | resource |
| [aws_s3_bucket_public_access_block.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_public_access_block)                                   | resource |
| [aws_s3_bucket_server_side_encryption_configuration.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_server_side_encryption_configuration) | resource |
| [aws_s3_bucket_versioning.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket_versioning)                                                     | resource |
| [random_id.bucket_suffix](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/id)                                                                          | resource |

## Inputs

| Name                                                                                 | Description                                                      | Type     | Default | Required |
| ------------------------------------------------------------------------------------ | ---------------------------------------------------------------- | -------- | ------- | :------: |
| <a name="input_add_random_suffix"></a> [add_random_suffix](#input_add_random_suffix) | Set to true to add a random suffix to the bucket name.           | `bool`   | `true`  |    no    |
| <a name="input_bucket_name"></a> [bucket_name](#input_bucket_name)                   | The desired name for the S3 bucket.                              | `string` | n/a     |   yes    |
| <a name="input_public_access"></a> [public_access](#input_public_access)             | Set to true to make the bucket public, false to keep it private. | `bool`   | `false` |    no    |

## Outputs

| Name                                                           | Description                                     |
| -------------------------------------------------------------- | ----------------------------------------------- |
| <a name="output_bucket_id"></a> [bucket_id](#output_bucket_id) | The unique identifier of the created S3 bucket. |

<!-- END_TF_DOCS -->
