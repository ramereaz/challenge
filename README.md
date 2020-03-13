# challenge
challenge by contino

# Command to be used to create the required stack

# Above script will take 3 parameters 

1+ Stack name
2+ MyName: 
    Type: String
    Description: Name of the Candidate
    Default: RamezElkomos
    
3+ Mobilenum:
    Type: String
    Description: Mobile number to receive message of any item added to the table format simlar to the following +61421345678
    Default: +61421762395
 
# Above cloudformation script will create the following resources
Resources:
  DynamoDB Table: Challenge_${MyName}
  SNS Topic: ItemAdded
  Lambda Function:
  IAM Role
  ApiRestApi: RestTechChallenge1_${MyName}
  
