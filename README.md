# Terraform AWS VPC and EC2: Effortless Deployment of a Secure and Scalable 3-Tier Architecture on AWS

---

## Architecture Diagram

![Terraform AWS VPC and EC2 - Architecture](/architecture-diagram/k8s-aws-architecture-v18082023-AWS%20VPC%20-%20EC2%20Instance%20-%20Security%20Groups.png)

---

## Introduction

Welcome to the Terraform AWS VPC and EC2 repository – your one-stop solution for effortlessly deploying a robust 3-tier architecture on Amazon Web Services (AWS) using the power of Terraform. Whether you're an infrastructure enthusiast, a DevOps engineer, or a cloud architect, this repository is designed to simplify the deployment process and help you establish a secure, scalable, and high-performance environment in no time.

Our curated workflow leverages Terraform's declarative approach to infrastructure as code, enabling you to create a Virtual Private Cloud (VPC) with Web, App, and Database tiers seamlessly. With pre-configured AWS Security Group modules, your setup will be fortified with well-defined inbound rules, ensuring the right balance between accessibility and security.

Deploying multiple EC2 instances in private subnets for your application, along with a dedicated Bastion Host in a public subnet, has never been easier. The repository includes automation for attaching Elastic IPs to the Bastion Host, streamlining remote access to your private instances.

But that's not all – we take it a step further by integrating null_resource with a duo of Terraform Provisioners: the File Provisioner and the Remote-exec Provisioner. These tools give you the flexibility to initialize instances with the right configurations and execute remote commands effortlessly, saving you time and manual effort.

Whether you're a seasoned cloud veteran or just starting your cloud journey, the Terraform-AWS-3Tier-VPC repository empowers you to architect, deploy, and manage a top-notch infrastructure on AWS with finesse. Let's elevate your cloud game together!

---

## Problem Statement and Solution

---

## Terraform Commands

### Terraform Initialize

```shell
terraform init
```

---

### Terraform Validate

```shell
terraform validate
```

---

### Terraform plan

```shell
terraform plan
```

---

### Terraform Apply

```shell
terraform apply
```

---

### Terraform Destroy

```shell
terraform apply -destroy -auto-approve
```

---
