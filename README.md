# Deploy a high availability web app using CloudFormation

In this project, you’ll deploy web servers for a highly available web app using CloudFormation.

## Installation

* Install [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)
* Create a S3 Bucket and add index.html file
* Create stack of network and servers
```
./create.sh CB-Udacity-Network network.yml network-parameters.json
./create.sh CB-Udacity-Servers servers.yml server-parameters.json
```

## Outputs

In the tab Output AWS Console -> CloudFormation -> CB-Udacity-Servers is possible to see the endpoint of the application
