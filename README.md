# Terraform Beginner Bootcamp 2023

## Project Description

![TerraTowns](screenshots/Screenshot%202023-09-24%20at%201.30.19%20PM.png)

TerraTowns is a community website that acts as a hub to discover and connect terraformers to each other's self-hosted personal websites in the style of Geocities of 2023.

Terraformers will write the infrastructure as Code (IaC) to launch their Terra House.
A Terra House is a simple Content Management System (CMS) that will allow you to author your own personal website and connect it to the TerraTowns network.

[Project Documents](https://docs.google.com/document/d/1Ywh-7qaMz3FHUK6SlpZaXJd__FYQnwIlq8MaRmP_X_M/edit#heading=h.gsr323tdunxb)

## System Design
![SysDesign](/screenshots/Screenshot%202023-09-24%20at%205.50.21%20PM.png)

### Semantic Versioning:
This project is using semantic versioning for it's tagging.

[semantic versioning docs](https://semver.org/)

Format:
 **MAJOR.MINOR.PATCH** eg `1.0.1`:

- **MAJOR** version when you make incompatible API changes
- **MINOR** version when you add functionality in a backward compatible manner
- **PATCH** version when you make backward compatible bug fixes

## References
**[Terraform CLI Installation](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)**
>Terraform CLI is installed for the project using a bash script [./bin/install-terraform-cli.sh](./bin/install-terraform-cli.sh)

### Working with environment variables
- To list out all environment variables, use the `env` command
- To filter specific environment variables use the `grep` command piped with the `env` command
- To set an environment variable use `export hello='Hello World'`
- To unset and environment variable use `unset hello`
- When using environment variables in a bash script they can be set without using `export`
- To print an environment variable use `echo $hello`
- To persist environment variable across gitpod workspace use `gp env hello='Hello World'`

**[AWS CLI Installation](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)**

> AWS CLI is installed for the project using a bash script [./bin/install-aws-cli.sh](./bin/install-aws-cli.sh)

**[AWS CLI Environment Variables](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html)**

 > To check if  credentials were configured correctly run ```aws sts get-caller-identity```

 ### Terraform Basics
 - Terraform Registry
    - Providers
    - Modules