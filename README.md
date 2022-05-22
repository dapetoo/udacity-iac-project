# Project Title - Deploy a high-availability web app using CloudFormation

This project contains files to provision infrastructure for a web application on AWS using AWS CloudFormation service.

## File Structure

### network-infrastructure-configutation.yml and network-parameters.json

Are used in provisioning the network infrastructure such as the VPC, Subnets, Route Table, ElasticIP, NatGateway etc and can be created using the below commands.

``` aws cloudformation create-stack --stack-name Network-Infrastructure-Stack --template-body file://network-infrastructure-configuration.yml --parameters file://network-parameters.json  
```

### server-infrastructure-configutation.yml and server-parameters.json

Are used in provisioning the server infrastructure such as the LaunchConfiguration, AutoScaling, LoadBalancer etc and can be created using the below commands.

``` aws cloudformation create-stack --stack-name Network-Infrastructure-Stack --template-body file://server-infrastructure-configuration.yml --parameters file://server-parameters.json
```

