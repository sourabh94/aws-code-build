# Building terraform code with AWS CodeBuild

Tested successfully with Amazon Linux container images

Update version in the following line for terraform package installation, in this case version 1.3.9 is used : 
```
curl -s -qL -o terraform_install.zip https://releases.hashicorp.com/terraform/1.3.9/terraform_1.3.9_linux_amd64.zip
```

We can pass environment variable in code build, $TF_CMD to apply or destroy changes :
```
terraform $TF_CMD --auto-approve
```

Please note the test was performed with S3 as backend and lock file was stored in DynamoDB, follow link for complete blog :
<https://www.ioconnectservices.com/insight/aws-with-terraform>

