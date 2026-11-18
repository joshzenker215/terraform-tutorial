# Terraform Tutorial
I'm learning Terraform from the official Hashicorp tutorial. I will be deploying to AWS.

## How to Initialize AWS CLI
I followed the recommendations in the AWS documentation. They assume you have already created an IAM user with PowerUser permissions.
1. Use the SSO wizard to create a default profile
1. Each time you want to start a session, run `aws sso login`
1. Run `aws configure list` to see your credentials