ecs-cloudformation
====

## How to use
### Attach policies
- AmazonEC2ContainerRegistryFullAccess
- AmazonEC2ContainerServiceFullAccess
- AmazonS3ReadOnlyAccess
- AmazonVPCFullAccess
- AWSCloudFormationFullAccess

### Create S3 bucket.

### Clone Repository and Edit stacks.yml
- Edit bucket name.
- Upload all files to S3.
```
aws s3 cp ./ s3://{bucket_name}/sample/ --recursive --exclude "*" --include "*.yml" --profile private
```
- Create stack on AWS Console.
