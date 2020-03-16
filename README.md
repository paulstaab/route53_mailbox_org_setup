# route53_mailbox_org_setup

CloudFormation template for using mailbox.org as email provider for a domain hosted in AWS Route53

## Usage

- Create a new `template.json` based on `template-example.json` and adjust your parameters, most importantly your domain name
- Create a new CloudFormation stack with
```
aws cloudformation create-stack --stack-name <StackName> --template-body file://dns_email_mailbox_org.yaml --parameters file://parameters.json
```

Thats it.

## Update the stack later
To update the stack, use
```
aws cloudformation update-stack --stack-name <StackName> --template-body file://dns_email_mailbox_org.yaml --parameters file://parameters.json
```

