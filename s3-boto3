import requests
import boto3
from botocore import UNSIGNED
from botocore.client import Config

s3 = boto3.client("s3", config=Config(signature_version=UNSIGNED))

mybucket = s3.list_objects(Bucket="bucketname")['Contents'] #add bucketname here

for files in mybucket:
    print(files["Key"])
