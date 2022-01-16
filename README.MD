# About Project
1-vpc
<br />
2-subnets
<br />
  a-
  <br />
    • NAT gateway
    <br />
    • Private VM
    <br />
  b-
    Private standard GKE cluster
    
# Project Google Cloud Plateform

project google cloud terraform with docker

## Installation-Terraform

to install it run this commands

```bash
terraform init
```
```bash
terraform plan
```
```bash
terraform apply
```
## Installation-Docker

to install it run this commands

```bash
docker build -t image-name .
```
If you want pull image to docker hub

```bash
docker push -account-name/repo-name:image-tag
```
If you want pull image to gcr

```bash
docker tag image-tag gcr.io/project-id/image-name
```
```bash
gcloud auth configure-docker
```
```bash
docker tag tag-name gcr.io/abdelrahman-adel/image-name
```
```bash
docker push gcr.io/project-id/image-name
```
