# Terraform AWS VPC and EC2: Effortless Deployment of a Secure and Scalable 3-Tier Architecture on AWS

![Terraform AWS VPC and EC2 - Architecture](/architecture-diagram/YT-Thumbnail- AWS%20VPC,%20EC2,%20Bastion%20Hosts,%20Security%20Groups%20Terraform.png)

---

## Architecture Diagram

![Terraform AWS VPC and EC2 - Architecture](/architecture-diagram/k8s-aws-architecture-v18082023-AWS%20VPC%20-%20EC2%20Instance%20-%20Security%20Groups.png)

---

## Introduction

Welcome to the Terraform AWS VPC and EC2 repository – your one-stop solution for effortlessly deploying a robust 3-tier architecture on Amazon Web Services (AWS) using the power of Terraform. Whether you're an infrastructure enthusiast, a DevOps engineer, or a cloud architect, this repository is designed to simplify the deployment process and help you establish a secure, scalable, and high-performance environment in no time.

Our curated workflow leverages Terraform's declarative approach to infrastructure as code, enabling you to create a Virtual Private Cloud (VPC) with Web, App, and Database tiers seamlessly. With pre-configured AWS Security Group modules, your setup will be fortified with well-defined inbound rules, ensuring the right balance between accessibility and security.

Deploying multiple EC2 instances in private subnets for your application, along with a dedicated Bastion Host in a public subnet, has never been easier. The repository includes automation for attaching Elastic IPs to the Bastion Host, streamlining remote access to your private instances.

But that's not all – we take it a step further by integrating null_resource with a duo of Terraform Provisioners: the File Provisioner and the Remote-exec Provisioner. These tools give you the flexibility to initialize instances with the right configurations and execute remote commands effortlessly, saving you time and manual effort.

Whether you're a seasoned cloud veteran or just starting your cloud journey, this repository empowers you to architect, deploy, and manage a top-notch infrastructure on AWS with finesse. Let's elevate your cloud game together!

---

## Problem Statement and Solution

**Problem Statement:**
Deploying a secure and scalable 3-tier architecture on cloud infrastructure is a complex task, often involving multiple manual steps, potential security vulnerabilities, and considerable time investment. Coordinating the creation of Virtual Private Clouds (VPCs), managing security groups, provisioning instances, setting up a Bastion Host, and ensuring proper configuration across the tiers can be daunting, error-prone, and resource-intensive. This process demands a solution that streamlines and automates these tasks while maintaining a strong focus on security and efficiency.

**Solution:**
Introducing the Terraform AWS VPC and EC2 GitHub repository – your comprehensive solution for effortlessly setting up a robust 3-tier architecture on Amazon Web Services (AWS) using the power of Terraform. This repository provides a streamlined and automated workflow that addresses the challenges of manual deployments and security concerns.

With the provided Terraform scripts, you can create a VPC with three distinct tiers – Web, App, and DB – each residing in its private subnet, ensuring separation of concerns and enhancing security. The included AWS Security Group Terraform module defines essential inbound rules, such as allowing HTTP port 80 and SSH port 22 access from the entire internet (0.0.0.0/0), while maintaining a balance between accessibility and security.

The heart of this solution lies in the automated deployment of multiple EC2 instances across the VPC's private subnets. These instances are provisioned with the necessary software and configurations, saving you valuable time and effort. Additionally, the repository facilitates the creation of a dedicated EC2 instance acting as a Bastion Host in a public subnet, enhancing your remote access capabilities.

To simplify remote management and configuration, the repository incorporates a null_resource with two Terraform Provisioners – File Provisioner and Remote-exec Provisioner. These tools empower you to efficiently initialize instances with required files and execute remote commands, all seamlessly integrated into your deployment process.

Say goodbye to complex manual setups and potential security gaps. This repository empowers you to architect, deploy, and manage a secure and scalable 3-tier architecture on AWS with ease, making your cloud infrastructure journey efficient, secure, and hassle-free.

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
