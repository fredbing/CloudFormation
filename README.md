# CloudFormation
My YAML files for AWS CloudForamtion templates

# S3 static website

# EC2 instance
In this YAML file, the KeyName under "MyEC2Instance" must be the Name of an existing EC2 KeyPair in the same region where the EC2 instance is to be created, though the KeyName in this example is not real.

The GroupName under "InstanceSecurityGroup" must be a new security group, therefore, it cannot be the same as any existing security group.

# Kinesis Stream
