# Building docker images
For building docker images using AWS CodeBuild

update the account-id and repository name in following lines : 

      - aws ecr get-login-password --region $AWS_DEFAULT_REGION | docker login --username AWS --password-stdin account-id.dkr.ecr.ap-south-1.amazonaws.com
      - REPOSITORY_URI=account-id.dkr.ecr.ap-south-1.amazonaws.com/repo
