# challenge
challenge by contino


# Steps to create required stack
== Through the console
1+ Open aws console and navigate to cloudformation service
2+ Click on "create stack"
   1- choose creating new resources
   2- upload the template script file "cf-template_ver1.yaml"

== Through the command line
aws cloudformation create-stack --stack-name challengestack --template-body file://cf-template_ver1.yaml --parameters ParameterKey=MyName,ParameterValue=RamezElkomos ParameterKey=Mobilenum,ParameterValue=+61421762395

# Above script will take 3 parameters 

1+ MyName: 
    Type: String
    Description: Name of the Candidate
    Default: RamezElkomos
    
2+ Mobilenum:
    Type: String
    Description: Mobile number to receive message of any item added to the table format simlar to the following +61421345678
    Default: +61421762395
 
# Above cloudformation script will create the following resources
  DynamoDB Table: Challenge_${MyName}
  SNS Topic: ItemAdded
  Lambda Function:
  IAM Role
  ApiRestApi: RestTechChallenge1_${MyName}
  

  
