# spring-rds-example
Simple spring application with spring aws cloud

## Usage


## Deploy
### Create
```
aws cloudformation create-stack --capabilities CAPABILITY_IAM --stack-name todo-app --template-body file://cfn.yaml --parameters ParameterKey=SoftwareVersion,ParameterValue=latest ParameterKey=RdsPassword,ParameterValue=<RDS_PASSWORD>
```

### Update
```
aws cloudformation update-stack --capabilities CAPABILITY_IAM --stack-name todo-app --template-body file://cfn.yaml --parameters ParameterKey=SoftwareVersion,ParameterValue=latest ParameterKey=RdsPassword,ParameterValue=<RDS_PASSWORD>
```