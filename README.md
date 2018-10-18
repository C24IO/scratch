# scratch
Small python utils

This worked - 

Run this in Cloud9 IDE 

#!/usr/bin/env python

import boto3

s3Client = boto3.client('s3')

print("URL \n\n\n{} \n\n\n\n".format(s3Client.generate_presigned_url('get_object', Params = {'Bucket': 'chazarey-public-share', 'Key': 'Deck.pdf'}, ExpiresIn = 21600)))



