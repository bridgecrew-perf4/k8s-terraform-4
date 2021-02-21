https://learn.hashicorp.com/tutorials/terraform/eks

Project Title
=====================
Terraform is used to provision and manage IT Infrastructure

Pre-Requisites
============================



Execution Flow
=====================

$git clone https://github.com/cloudstones/k8s-terraform.git

$cd k8s-terratform/src

$terraform init .

$terraform apply .

configure kubectl

aws eks --region $(terraform output -raw region) update-kubeconfig --name $(terraform output -raw cluster_name)
