acceptance-test-composite
============================


## Description
This is the CloudCoreo acceptance test composite


## Hierarchy
![composite inheritance hierarchy](https://raw.githubusercontent.com/CloudCoreo/acceptance-test-composite/master/images/hierarchy.png "composite inheritance hierarchy")



## Required variables with no default

### `TOMCAT_KEYPAIR`:
  * description: 


## Required variables with default

### `VPC_NAME`:
  * description: the name of the VPC
  * default: acceptance-test-vpc


### `VPC_OCTETS`:
  * description: the /16 net of the VPC to look for - i.e 10.11.0.0
  * default: 10.66.0.0


### `REGION`:
  * description: use default except for multiple region use cases
  * default: PLAN::region

### `PRIVATE_ROUTE_NAME`:
  * description: the name to give to the private route
  * default: acceptance-test-private-route


### `PRIVATE_SUBNET_NAME`:
  * description: the cloudcoreo name of the private vpc subnets
  * default: acceptance-test-private-subnet


### `PUBLIC_ROUTE_NAME`:
  * description: the name to give to the public route
  * default: acceptance-test-public-route


### `PUBLIC_SUBNET_NAME`:
  * description: the cloudcoreo name of the public vpc subnets
  * default: acceptance-test-public-subnet


### `PUBLIC_SUBNET_NUM_ZONES`:
  * description: the number of public subnet zones
  * default: 1

### `AUDIT_AWS_CLOUDTRAIL_ALERT_LIST`:
  * description: Which alerts would you like to check for? (Default is all Cloudtrail alerts)
  * default: cloudtrail-service-disabled, cloudtrail-no-global-trails, cloudtrail-inventory, cloudtrail-trail-with-global

### `AUDIT_AWS_CLOUDTRAIL_ALLOW_EMPTY`:
  * description: Would you like to receive empty reports? Options - true / false. Default is false.
  * default: true

### `AUDIT_AWS_CLOUDTRAIL_SEND_ON`:
  * description: Send reports always or only when there is a change? Options - always / change. Default is change.
  * default: change

### `AUDIT_AWS_CLOUDTRAIL_REGIONS`:
  * description: List of AWS regions to check. Default is us-east-1,us-east-2,us-west-1,us-west-2,eu-west-1.
  * default: us-east-1, us-east-2, us-west-1, us-west-2, eu-west-1

### `AUDIT_AWS_CLOUDTRAIL_ROLLUP_REPORT`:
  * description: Would you like to send a rollup Cloudtrail report? This is a short email that summarizes the number of checks performed and the number of violations found. Options - notify / nothing. Default is nothing.
  * default: nothing

### `AUDIT_AWS_CLOUDTRAIL_HTML_REPORT`:
  * description: Would you like to send a full Cloudtrail report? This is an email that details any violations found and includes a list of the violating cloud objects. Options - notify / nothing. Default is nothing.
  * default: nothing

### `TOMCAT_GROUP_MAXIMUM`:
  * description: Minimum number of instances the autoscale group will launch
  * default: 1

### `TOMCAT_GROUP_MINIMUM`:
  * description: Maximum number of instances the autoscale group will launch
  * default: 1

### `TOMCAT_INGRESS_CIDRS`:
  * description: 
  * default: 0.0.0.0/0

### `TOMCAT_INGRESS_CIDR_PORTS`:
  * description: 
  * default: 1f90, 50, 1bb, 16

### `TOMCAT_INGRESS_GROUP_PORTS`:
  * description: 
  * default: 1f90, 50, 1bb

### `TOMCAT_NAME`:
  * description: 
  * default: ac-cat


### `TOMCAT_SIZE`:
  * description: 
  * default: t2.micro


### `VPC_CIDR`:
  * description: The CIDR to match to locate the VPC that this server is to be created in
  * default: 10.66.0.0/16


## Optional variables with default

### `VPC_TAGS`:
  * description: tags to apply to the vpc
  * default: acceptance-test

### `AUDIT_AWS_CLOUDTRAIL_OWNER_TAG`:
  * description: Enter an AWS tag whose value is an email address of the owner of the Cloudtrail object. (Optional)
  * default: NOT_A_TAG


## Optional variables with no default

### `SUFFIX`:
  * description: when used will use the value to suffix the names of all converged objects

### `AUDIT_AWS_CLOUDTRAIL_ALERT_RECIPIENT`:
  * description: Enter the email address(es) that will receive notifications. If more than one, separate each with a comma.

### `YUM_REPO_BUCKET`:
  * description: 

## Tags
1. Testing
1. Acceptance_Test


## Categories
1. Testing



## Diagram
![diagram](https://raw.githubusercontent.com/CloudCoreo/acceptance-test-composite/master/images/diagram.png "diagram")


## Icon


