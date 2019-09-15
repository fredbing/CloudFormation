# CloudFormation
My YAML files for AWS CloudForamtion templates

# S3 static website

# EC2 instance
In the "ec2_instance_sshkey" file, the KeyName (with ".pem" being removed) is embedded in "MyEC2Instance". Embeddinbg keyname is not the recommened best practice but a straightforward way to do. Keep in mind that the name of the existing EC2 KeyPair provided must be in the same region where the EC2 instance is to be created (the KeyName here is only an example and is not a real key).
The GroupName under "InstanceSecurityGroup" must be a new security group, therefore, it cannot be the same as any existing security group.

In the "ec2_instance_2" file, the SSH is passed as an parameter. Note that it needs to provide the Default value for the key, e.g.: "Default: bigdatakey". Two regions I use most frequently: us-east-1 and us-west-2 are included in the mapping paratmeters. The instance will be created in the region in which the SSH keyname is associated with. SG name is assigned when instance is created, as compared with the "ec2_instance_sshkey" file where the SG name is given in the code. 

# Kinesis Stream
