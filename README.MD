# Project Google Cloud Plateform

project google cloud terraform with docker

# About Project
<h4>1-vpc</h4>
<h4>2-subnets</h4>
<ul>
    <p>a-</p>
        <ul>
            <li>
                <p>NAT gateway</p>
            </li>
            <li>
                <p>Private VM</p>
            </li>
        </ul>
</ul>
<ul>  
    <p>b-</p>
        <ul>
            <li>
                <p>Private standard GKE cluster</p>
            </li>
        </ul>
</ul>

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
docker tag image-id profile-name/repo-name:image-name
```
```bash
docker push -account-name/repo-name:image-tag
```

If you want pull image to gcr

```bash
gcloud auth configure-docker
```
```bash
docker tag tag-name gcr.io/abdelrahman-adel/image-name
```
```bash
docker push gcr.io/project-id/image-name
```
