#!/bin/bash
#(for osx not linux)

# Howdy
# lets get cracking


aws --region us-west-2 --profile default iam list-server-certificates
aws ec2 list-server-instances

echo "more stuff here"
#whatever

# or  for python:
# import boto3
# import datetime
# default=boto3.session.Session(profile_name='default')
# ec2 = default.resource('ec2', region_name='us-west-2')
# or my_instances = ec2.describe-instances()
### look at filtering here: http://boto3.readthedocs.io/en/latest/guide/migrationec2.html

# or setup connection and
# iam = default.recource('iam')
### no regions for iam but there are for acm!
# my_certificates = list-server-certificates()

### don't forget that for cloudfront all certs are stored in us-east-1
