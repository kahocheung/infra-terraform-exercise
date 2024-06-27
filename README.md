## Objective:

You are provided with a GitHub branch containing Terraform code for a 3-tier application setup on AWS. This architecture encompasses an Application Load Balancer (ALB), an Elastic Container Service (ECS) instance running a WordPress application, and a Relational Database Service (RDS) with MySQL set up in a Virtual Private Cloud (VPC). However, there are known issues in the VPC provisioning and configuration, as well as problems in the provisioning of the 3-tier system itself.

## Review and Debug:
Start by cloning the provided GitHub branch.

Examine the Terraform code for any errors, misconfigurations, or missing resources related to the VPC and the 3-tier application setup

Note: The VPC/network configurations are located in a separate directory.

## Fix and deploy the VPC along with the rest of the networking configuration:
Before moving to the application setup, ensure the VPC and associated network configurations are fixed and correctly provisioned.
Ensure that the setup allows for instances setup in the private subnets to have access to the public internet.

You are allowed and encouraged to run terrafrom plans and terraform apply for the VPC to validate your fixes.

## Fix and deploy the 3-Tier Application Setup:
After ensuring the VPC is correctly provisioned, move on to fixing the 3-tier application setup.

Modify the Terraform code to address and fix the identified issues, ensuring that your code sets up the application correctly and handles any dependencies between resources.
 
The resources should be deployed within the VPC created earlier.
The RDS instance and the ECS application should be provisioned within private subnets, ensuring they are not directly accessible from the public internet but can still communicate with other necessary AWS services.


## Final Deployment:
Your final Terraform code should be ready for deployment.
When we run terraform apply, the entire infrastructure, including VPC, ALB, ECS with WordPress, and RDS with MySQL, should spin up correctly without errors.


## Evaluation Criteria:
Quality of the fixed code

Ability to identify and resolve issues in a systematic manner (VPC first, followed by the application setup)

Successful deployment of the VPC and the 3-tier application

We're looking for your ability to navigate complex infrastructure code, troubleshoot effectively, and deliver a robust solution in the correct order of operations. Best of luck!
