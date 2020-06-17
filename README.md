# Deploy a high availability web app using CloudFormation

In this project, you’ll deploy web servers for a highly available web app using CloudFormation.

## Installation

* Install [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)
* Create a S3 Bucket and add index.html file
* Give execution permission to _create.sh_ and _update.sh_
```
chmod +x create.sh
chmod +x update.sh
```
* Create stack of network and servers
```
./create.sh CB-Udacity-Network network.yml network-parameters.json
./create.sh CB-Udacity-Servers servers.yml server-parameters.json
```

## Update

If you modify the code, you have to update the stack with the same parameters that using before

```
./create.sh CB-Udacity-Network network.yml network-parameters.json
```
or
```
./create.sh CB-Udacity-Servers servers.yml server-parameters.json
```

## Outputs

In the tab Output of AWS Console -> CloudFormation -> CB-Udacity-Servers is possible to see the endpoint of the application
