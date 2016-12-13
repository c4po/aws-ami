##
Build RHEL 7 ami with docker

## Build Mode
create vars/aws_variables.json from vars/aws_variables.json.tmpl with valid credentials
```
packer build -var-file=./vars/aws_variables.json [NAME].json
```
### Debug Mode
```
packer build --debug -var-file=./vars/aws_variables.json [NAME].json
```

### AMI BUILDER (EBS BACKED) doc
https://www.packer.io/docs/builders/amazon-ebs.html

### AWS create-image cli doc
http://docs.aws.amazon.com/cli/latest/reference/ec2/create-image.html

