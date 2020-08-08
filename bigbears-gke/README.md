# How to create GKE with Terraform script
## Setup Google Cloud credentials
```
export GOOGLE_APPLICATION_CREDENTIALS=[/patgh/to/google/service/account/json 
```

## Declare terraform variable values in "terraform.tfvars"
```
project_id   = "bigbears-io"                     # Put GCP Project ID.
machine_type = "n1-standard-1"        # Put the desired VM Instance type.
cluster_name = "bigbears-gke"
```

## Terraform init / plan / apply
```
$ terraform init
$ terraform plan --out 1.plan
$ terraform apply 1.plan
```