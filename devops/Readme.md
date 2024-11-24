1. When writing Terraform code, how many spaces between each nesting level does HashiCorp recommend that you use?
ANS: 2

2. How to Define Env Variable.
ANS: TF_VAR

3. Provider dependencies are created in several different what are those.
ANS:
Explicit use of a provider block in configuration, optionally including a version constraint. 
Existence of any resource instance belonging to a particular provider in the current state.
Use of any resource block or data block in the configuration, belonging to a particular provider

4. which of the following are valid provider versions that satisfy the expression 

terraform {
  required_providers {
    aws = {
      source = "hashicorp/aws"
      version ~> "5.6.0"
    }
  }
}

ANS: ANY THING IN RANGE OF (5.69.0 TO 5.69.9)

5. Why a user opt to include the terraform version in configuration file?

ANS: The user wants to specify the minimum version of Terraform that is required to run the configuration

6. When multiple arguments with single-line values appear on consecutive lines at the same nesting level, HashiCorp recommends that you:

ANS: align the equals signs
     ami           = "abc123" 
     instance_type = "t2.micro"

7. TERRAFORM RUNS ON WHICH OS 

LINUX
WINDOWS
MACOS
SOLARIS
FREEBSD
AIX(WILL NOT SUPPORT)

8. True or False? Using the latest versions of Terraform, terraform init cannot automatically download community providers.
ANS: FALSE


9. If I have aws and azure provider and run init command where provider plugins will store.
ANS: .terraform/providers directory in the current working directory

10. when we have duplicate provier blocks what we need to use.
ANS: ALIAS

11. While Terraform is generally written using the HashiCorp Configuration Language (HCL). What other syntax can Terraform be expressed in?

ANS: JSON

12. What feature of Terraform can execute a script on the remote server once is has been provisioned?
ANS: remote-exec provisioner

13. A provider block is required in every configuration file so Terraform can download the proper plugin.
ANS: False

14. You need to define a single input variable to support the IP address of a subnet, which is defined as a string, and the subnet mask, which is defined as a number. What type of variable variable should you use?
ANS: type = object ()

15. Which of the following Terraform versions would be permitted to run the Terraform configuration based on the following code ?

terraform {
  required_version = "~> 5.0.0"
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 3.0"
    }
    random = {
      source  = "hashicorp/random"
      version = "3.1.0"
    }
  }
}

ANS: 

Terraform v5.2.0 
Terraform v5.0.5 : TRUE
Terraform v5.4.9
Terraform v5.1.0

16. You are using Terraform to manage some of your AWS infrastructure. You notice that a new version of the provider now includes additional functionality you want to take advantage of. What command do you need to run to upgrade the provider?

ANS: terraform init -upgrade


17. How to download a specific version of the AWS provider?

18. You have recently cloned a repo containing Terraform that you want to test in your environment. Once you customize the configuration, you run a terraform apply but it immediately fails. Why would the apply fail?
ANS: Terraform needs to initialize the directory and download the required plugins


19. When developing Terraform code, you must include a provider block for each unique provider so Terraform knows which ones you want to download and use.
ANS: FALSE

20. When using Terraform, where can you install providers from? (select four)
ANS:
Terraform plugin cache : TRUE
official HashiCorp releases site : TRUE
Terraform registry : TRUE
the provider's source code : FALSE
plugins directory : TRUE

21.  Running a terraform fmt will modify Terraform configuration files in the current working directory and all subdirectories.
ANS: FALSE

22. You need to use multiple resources from different providers in Terraform to accomplish a task. Which of the following can be used to configure the settings for each of the providers?

provider "consul" {
  address = "https://consul.raham.com:8500"  
  namespace = "developer"
  token = "6383iehe743-07c7-47a4-52fd-ge3y78eijrd"
}
 
provider "vault" {
  address = "https://vault.raham.com:8200"
  namespace = "developer"
}

23. What feature of Terraform provides an abstraction above the upstream API and is responsible for understanding API interactions and exposing resources?
ANS: Terraform provider

24. True or False? A main.tf file is always required when using Terraform?
ANS: FALSE

25. A provider alias is used for what purpose in a Terraform configuration file?
ANS: using the same provider with different configurations for different resources

26. Using the Terraform code below, where will the resource be provisioned?

provider "aws" {
  region = "us-east-1"
}
 
provider "aws" {
  alias  = "west"
  region = "us-west-2"
}
 
provider "aws" {
  alias  = "eu"
  region = "eu-west-2"
}
 
resource "aws_instance" "vault" {
  ami                         = data.aws_ami.amzlinux2.id
  instance_type               = "t3.micro"
}

ANS: 

us-west-1
us-west-2
us-east-1 : TRUE

27. CAN you can provide these credentials in resources block in your configuration ?
ANS: FALSE

28. Scenario: You are deploying a new application and want to deploy it to multiple AWS regions within the same configuration file. Which of the following features will allow you to configure this?
ANS: multiple provider blocks using an alias

29. Based on the Terraform code below, what block type is used to define the VPC?
vpc_id = aws_vpc.main.id

ANS: resource block

30. Which of the following Terraform files should be ignored by Git when committing code to a repo? (select two)
ANS: 

outputs.tf
terraform.tfstate  : TRUE
terraform.tfvars   : TRUE
variables.tf

31. Which of the following describes the process of leveraging a local value within a Terraform module and exporting it for use by another module?
ANS: Exporting the local value as an output from the first module, then importing it into the second module's configuration.

32. Before a new provider can be used, it must be ______ and _______. (select two)
ANS: 

approved by HashiCorp
initialized                 : TRUE
uploaded to source control
declared or used in a configuration file : TRUE

33. Why is it a good idea to declare the required version of a provider in a Terraform configuration file?
ANS:

terraform {
  required_providers {
    aws = {
      source = "hashicorp/aws"
      version = "3.57.0"
    }
  }
}

ANS: providers are released on a separate schedule from Terraform itself; therefore, a newer version could introduce breaking changes


34. In the terraform block, which configuration would be used to identify the specific version of a provider required?
ANS; required_providers

35. Which of the following is considered a Terraform plugin?
ANS: Terraform provider

36. True or False? Multiple providers can be declared within a single Terraform configuration file.
ANS: TRUE

37. a plugin that Terraform uses to translate the API interactions with the service or provider
ANS: TRUE

38. Which configuration block type is used to declare settings and behaviors specific to Terraform?
ANS: terraform block






