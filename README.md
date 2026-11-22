# Terraform Tutorial
I'm learning Terraform from the official Hashicorp tutorial. I will be deploying to AWS.

## How to Initialize AWS CLI
I followed the recommendations in the AWS documentation. They assume you have already created an IAM user with PowerUser permissions.
1. Use the SSO wizard to create a default profile
1. Each time you want to start a session, run `aws sso login`
1. Run `aws configure list` to see your credentials

## Terraform Tips
I'll jot down tips and tricks I pick up while working on the tutorial.
- Whenever you add a new module to your configuration, you will need to install it by re-initializing the workspace, e.g. `terraform init`.
- You can use the same module more than once by specifying the same source and version arguments, while giving each module block a unique name.