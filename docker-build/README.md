# Building docker images with AWS CodeBuild

For building docker images using AWS CodeBuild and pushing them to ECR repository in same account.

Update the account-id and repository-name in following lines : 

      - aws ecr get-login-password --region $AWS_DEFAULT_REGION | docker login --username AWS --password-stdin account-id.dkr.ecr.ap-south-1.amazonaws.com
      - REPOSITORY_URI=account-id.dkr.ecr.ap-south-1.amazonaws.com/repository-name
