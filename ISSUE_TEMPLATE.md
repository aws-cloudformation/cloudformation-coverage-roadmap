## Instructions for CloudFormation Coverage New Issues Template

Quick Sample Summary:
1. Title -> AWS::Service::Resource-Attribute-Existing Attribute
2. Scope of request -> AWS::Service::ResourceType::TheResource-ExistingAttribute supports A and B today, but not new C feature.
3. Expected behavior -> In Create, it should include this and this, like the console.  Also include tag creation, like the API allows.
4. Test case recommendation (optional) -> it should help me do X given existing Y (if applicable); it should/shouldn't change Z.
5. Links to existing API doc (optional) -> Updated API docs at https://example.com/api-new.html
6. Category tag (optional) -> Compute
7. Any additional context (optional)

Detailed Instructions to create a new issue here: (delete this text before you save your issue, to keep them as short as possible :) ). 

## 1. Title 
In the format AWS::Service::Resource-Attribute-Existing Attribute) 
Samples:
#### AWS::Service::NewResource
#### AWS::Service::ExistingResource-NewAttribute
#### AWS::Service::ExistingResource-ExistingAttribute-NewOption

We are hoping that the title makes it easy for others to scan it quickly in kanban board or issue list. 

## 2. Scope of request 
Whether a new API call requires a new attribute, or a new feature is supported and needs to be added to CloudFormation.  Be as descriptive as possible so that others can +1 your request if it applies to them.
Should fall into the following categories:

   a) new service support is desired
   b) new resource type for an existing service is desired
   c) new attribute for an existing resource is desired 
   d) new option for an existing attribute is desired 
   e) other coverage-related issue with the resource/attribute/option

Samples: 
#### AWS::Service::ResourceType::TheResource-ExistingAttribute supports A and B today, but not new C feature.
#### AWS::Service::ResourceType::TheResource-NewAttribute to turn feature F on or off, or pass parameter P to API.
#### AWS::Service::NewResourceType - can create resource via API, but not via CloudFormation

## 3. Expected behavior

Samples:
#### In Create, it should include this and this, like the console.  Also include tag creation, or another thing that should be combined.
#### in Update, change the attribute X, and it shouldn't require replacement, like the API. Should it require UpdateReplacePolicy?
#### Any particular or uncommon Delete behavior? What are the expected options?

Feel free to describe other desired and relevant implementation details. 

## 4. Suggest specific test cases

Samples:
#### Common use case: pass X and Y parameter as a string, or as a !Ref 
#### Test case recommendation: it should help me do X given existing Y (if applicable); it should/shouldn't change Z.
#### Other recommendations: ensure drift checks that X thing changed in a subsequent describe/list call

## 5. Helpful Links to speed up research and evaluation

Samples:
#### Updated API docs at https://example.com/api-new.html
#### Mentioned in twitter, reddit, stack overflow, etc. here: https://twitter.com/postid12345678
#### It would be great if it worked like this similar procedure: https://example.com/similar.html

## 6. Category (required) - Will help with tagging and be easier to find by other users to +1

Use the categories as displayed in the AWS Management Console (simplified):

1. Compute (EC2, ECS, EKS, Lambda...)
2. Storage (S3, EFS, Backup...)
3. DB (RDS, DynamoDB...)
4.  Networking & Content (VPC, Route53, API GW,...)
5. Management (CloudTrail, Config...)
6. Machine Learning (SageMaker, ...)
7. Analytics (Athena, EMR, Glue,...)
8. Security (IAM, KMS...)
9. Integration (MQ, SQS, SNS,...)
10. Developer Tools (CodeStar, ...)
11. Other (IoT, Migration, Budgets...)

## 7. Any additional context (optional)
