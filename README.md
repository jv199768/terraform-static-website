'Taken From: How to Create a simple static Amazon S3 website using Terraform

https://dev.to/aws-builders/how-to-create-a-simple-static-amazon-s3-website-using-terraform-43hc'

Cleanup
Run terraform destroy

Delete Cloud9 environment

Caveat to the link above: You would be only destroying six (6) resources as the URI for http://static-website-bucket-terraform.s3-website-us-east-1.amazonaws.com/ is the only resource created.
Otherwise, your upload to S3 of index.html and error.html would result in configuration drift. 

index.html: http://static-website-bucket-terraform.s3-website-us-east-1.amazonaws.com/index.html#
error.html: http://static-website-bucket-terraform.s3-website-us-east-1.amazonaws.com/error.html
