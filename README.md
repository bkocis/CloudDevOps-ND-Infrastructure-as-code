
# Description 

The code contains AWS Cloud Formation confioguration for creating an infrastructure of multiple EC2 instances, load balancer in a network of private and public subnets. The project is part of Udacity's CloudDevOps nanodegree. 


# Files:

Defining the resources for the network: 

- resources.yaml
- resources-parameters.json

Defining the computational instances:

- servers_final.yaml
- servers-final-parameters.json


# Running the code that build the cloud infrastructure

### 1. create the network and elements subnets, VPS, gateways, etc.

`bash create_stack.sh resources resources.yaml resources-parameters.json 

### 2. create the instances and the define the code for the installation inside the instances
bash create_stack.sh instances servers_final.yaml servers-final-parameters.json


### AMI of choice 
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/finding-an-ami.html

Select an AMI considering:

- Region

- operating system

- architecture: 32-bit (i386), 64-bit (x86_64), or 64-bit ARM (arm64)

- root device type: Amazon EBS or instance store

- provider (for example, Amazon Web Services)

- additional software (for example, SQL server)

Some AMI could still be incompatible; search for an adequate one can be made in the EC2, Image AMI search pane. 


