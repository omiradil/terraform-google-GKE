# Terraform google cloude project

## This Module Creates GKE Cluster

### Copy and paste below code and run:  
@ 
                                         - terraform init
                                         - terraform apply.

```
module "app" {
  source         = "../"
  project        = "kcahrzeljocmrous" # "replace with your own project ID"
  region         = "us-central1"
  zone           = "us-central1-c"
  cluster_name   = "my-gke-cluster"
  machine_type   = "e2-medium"
  node_count     = 1
  node_pool_name = "my-node-pool"
  preemptible    = true
}

```