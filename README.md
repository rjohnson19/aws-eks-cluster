# aws-eks-cluster
Production ready AWS Kubernetes cluster provisioned using Terraform

## Setup instructions

### Prerequisites
- AWS account with admin privileges
- AWS CLI installed and configured (aws configure)
- Terraform installed (latest version)
- kubectl installed
- Ansible installed
- Helm installed

### Deploy Infrastructure

```
terraform init
terraform plan
terraform apply
```


### Tearing Down
When done reviewing the results, be sure to tear down the infrastructure to avoid ongoing costs.
```
terraform destroy
```

## Why this matters
- Being able to deploy a production grade EKS cluster using Terraform avoids manual effort, human error, and ensures security and best practices are followed.
- Infrastructure as code is reviewable by humans, static code analysis, and AI, and will allow ongoing maintenance and upgrades of the cluster in a consistent fashion.
- Terraform is platform agnostic and some of these configurations can be carried over to other cloud providers if desired.

## Cost Estimates
- 1 EKS cluster with Standard Support, and 2 nodes with 2 vCPU each would cost approximately 131.40 USD per month.
- Use https://calculator.aws/#/ to estimate costs for different vCPU hours and additional cloud resources.