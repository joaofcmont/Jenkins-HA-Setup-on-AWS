# Jenkins-HA-Setup-on-AWS

<h2>For this Jenkins HA project, I have used the following DevOps Tools : </h2> 

    GitHub: Repository to store IaC
    Packer: To build Jenkins Controller and agent AMIs
    Ansible: To configure Jenkins controller and agent during the AMI building process
    Terraform: To provision AWS resources
    Python Boto3: To retrieve SSH public key from AWS parameter store.

<h2>Following are the AWS services used : </h2>

    IAM: To create IAM Role/Instance Profile for Jenkins Controller and Agent Nodes.
    EFS: To store Jenkins data
    AWS Parameter Store: To store SSH private and public keys as secrets to configure agents.
    Autoscaling Group: To deploy the Jenkins controller
    Application Load Balancer: To have a static DNS endpoint for the Jenkins controller instance running in the autoscaling group.
