# Terraform-beginner-bootcamp-2023

<img width="300px" src="https://github.com/NickGoko/terraform-beginner-bootcamp-2023/assets/61675328/066397d8-64d2-4ea2-9398-7b2ba63b5576">

## Week 0 Prerequisite Week & Project Prep

- **Why Terraform**

Learning Terraform is crucial for :cloud: cloud engineers because it empowers them to provision and manage cloud resources as code. 

This Infrastructure as Code (IaC) approach ensures consistency, scalability, and efficiency in cloud deployments. 

Terraform's versatility and support for multiple cloud providers make it a valuable skill for automating infrastructure and orchestrating complex cloud environments, ultimately streamlining operations and reducing manual errors.

. **Codeblocks**

> This code is written in HashiCorp Configuration Language (HCL) and is used to define AWS resources that will be created or managed by [Terraform](/https://terraform-docs.io/user-guide/introduction/) <sup>[1]</sup>

```terraform
provider "aws" {
  region = "us-east-1" # Change to your preferred AWS region
}

resource "aws_s3_bucket" "my_bucket" {
  bucket = "my-unique-bucket-name" # Choose a unique name
  acl    = "private"              # Access control settings
}
```

|Task 1 |Create Github Repo & write up some documentation using Github Flavored Markdown |
| --- | --- |
|Task 2 | Set up Gitlab |
|Task 3 | Set up Terraform Cloud |


- [x] Finish Task 1
- [x] Finish Task 2
- [ ] Finish Task 3

## Week  1 Getting Comfortable with Terraform and Terraform Cloud

|Task 4 | Create Terrahouse Module|
| --- | --- |
|Task 5 |Static Website Hosting |


- [ ] Finish Task 4
- [ ] Finish Task 5

- State management
- Changesets
- Launching and Stop a Gitpod Workspace
- Configuration launch scripts eg. .Gitpod.yml files
---
## Week 2 Launching and Connecting our Terra house to TerraTowns
|Task 6 |Setting up Terratowns |
| --- | --- |
|Task 7 | Terraform cloud and Multi Home Refactor |


- [ ] Finish Task 6
- [ ] Finish Task 7

## Reference 
- [Terraform getting started](https://app.terraform.io/app/getting-started) <sup>[1]</sup>
- [Github Flavored Markdown](https://github.github.com/gfm/#backtick-string) <sup>[2]</sup>
- [Gitlab Docs](https://docs.gitlab.com/) <sup>[3]</sup>

Use Control + Shift + m to toggle the tab key moving focus. Alternatively, use esc then tab to move to the next interactive element on the page.
No file chosen
Attach files by dragging & dropping, selecting or pasting them.
Editing terraform-beginner-bootcamp-2023/README.md at main · NickGoko/terraform-beginner-bootcamp-2023

