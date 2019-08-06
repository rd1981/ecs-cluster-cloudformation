# POC AWS Multiple Stacks with ECS

## Requirements

- AWS Account or AWS User

## Usage

Ejecutar en consola los siguientes comandos

```bash
aws cloudformation package --template TEMPLATE_LOCATION --s3-bucket S3_BUCKET_NAME --output-template packaged-cf.yml --region us-east-1

aws cloudformation deploy --template-file ./packaged-cf.yml --stack-name STACK_NAME --capabilities CAPABILITY_IAM --region us-east-1
```