# spring-rds-example
Simple spring application with spring aws cloud

## Usage
```
http get <ELB-address>
```

## Deploy
### Create
```
aws cloudformation create-stack --capabilities CAPABILITY_IAM --stack-name todo-app --template-body file://cfn.yaml --parameters ParameterKey=SoftwareVersion,ParameterValue=latest ParameterKey=RdsPassword,ParameterValue=<RDS_PASSWORD>
```

### Update
```
aws cloudformation update-stack --capabilities CAPABILITY_IAM --stack-name todo-app --template-body file://cfn.yaml --parameters ParameterKey=SoftwareVersion,ParameterValue=latest ParameterKey=RdsPassword,ParameterValue=<RDS_PASSWORD>
```

### Delete
```
aws cloudformation delete-stack --stack-name todo-app
```