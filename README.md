# Terraform Localstack Example
  * Localstack is a tool that runs on your local machine and emulates AWS API
  * The default port is 4566

 # To start localstack
  * localstack start

 # To stop localstack
  * localstack stop

 Make sure you have a working docker setup on your local.

 # To check the created EC2 instances
   **  aws --endpoint-url=http://localhost:4566 ec2 describe-instances

 # To check the created EC2 instances filtered version
   **aws --endpoint-url=http://localhost:4566 ec2 describe-instances --query "Reservations[].Instances[].InstanceId
