# terraform-google
## Terraform google cloude project

```
module "app" {
  source         = "../"
  project        = "kcahrzeljocmrous"
  region         = "us-central1"
  zone           = "us-central1-c"
  cluster_name   = "my-gke-cluster"
  machine_type   = "e2-medium"
  node_count     = 1
  node_pool_name = "my-node-pool"
  preemptible    = true
}

```