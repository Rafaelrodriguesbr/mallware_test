
# NiceAPP

### Description

- publish WEB application and API
Create autoscale and loadbalance in 2 instances

- Make an application vulnerability scanner to validate if there are any vulnerabilities in these images.

- Save the vulnerability scanner report in S3

- Enable cloudtraill and log file validation

- Enable AWS Config service

- Centralize vulnerability report access logs and cloudtraill logs in another bucket




### Requirements
- [Terraform](https://www.terraform.io/downloads.html)
- [AWS Account](https://aws.amazon.com/)
- [Amazon EC2 Key Pairs](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html)

### Architecture
![Architecture](https://user-images.githubusercontent.com/32931856/51339968-ead70780-1a74-11e9-9a31-fe0892b65e59.png)


### Running the project

- Clone the repository
```
git clone https://github.com/rafaelaceno/opstest

```
- Edit the `variables.tf` file with the SSH public key location 
- Edit the `variables.tf `file with the name of the VPC that will be used for this infrastructure
- Edit the `variables.tf` file with the name of bucket s3 that is located the project spring_bot.zip

- Execute terraform

```
terraform init
terraform plan
terraform apply

```

### Removing the entire environment

To remove all created machines and settings, simply execute the command

`terraform destroy`


