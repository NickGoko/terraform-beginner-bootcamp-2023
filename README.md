# Terraform-beginner-bootcamp-2023


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

## References
### Considerations with Terraform CLI changes
The Terraform CLI installations instructions have changed due to gpg keyring changes. So we need to refer to the new terraform CLI installations instructions via terraform documentation. And change the scripting for install. 

[Install Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

### Refactoring into Bash Scripts
While fixing the terraform depreciation issues. We realised the install instructions had to many steps. So we decided to create a bash script to install the terraform CLI. Bash scripit is located at ([./bin/install_terraform_cli.sh](./bin/install_terraform_cli.sh))

- This will keep the gitpod task file tidy([.gitpod.yml](.gitpod.yml)). 
- This wil allow better portability for other projects that need terraform CLI. 
### Considerations for Linux distribution
This project is built against Ubuntu
Please consider check your linux distrubution and change according to your distrubution needs. 
([Check your linux distribution](https://www.cyberciti.biz/faq/find-linux-distribution-name-version-number/))
Example of checking OS version
```sh
$ cat /etc/*-release
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=22.04
DISTRIB_CODENAME=jammy
DISTRIB_DESCRIPTION="Ubuntu 22.04.3 LTS"
PRETTY_NAME="Ubuntu 22.04.3 LTS"
NAME="Ubuntu"
VERSION_ID="22.04"
VERSION="22.04.3 LTS (Jammy Jellyfish)"
VERSION_CODENAME=jammy
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=jammy
```
### Gitpod lifecyle (Before, init, command)
We need to be careful when using the Init in our .yml file because it will not rerun if we restart an existing workspace. 

[Gitpod Lifecycle](https://www.gitpod.io/docs/configure/workspaces/tasks)
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

