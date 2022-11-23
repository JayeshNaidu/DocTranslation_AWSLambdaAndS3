# DocTranslation_AWSLambdaAndS3
Translation of documents using AWS Lambda and S3

#Steps 
1. Create 2 buckets for input and output respectively.
2. Create a lambda role that has full access for s3, translate and cloudwatch.
3. Create a trigger for the function and attach the input bucket.
4. copy paste the code, remember to change the output bucket name to your output bucket name in following places:
  i. var outfile
  ii. Parameter(Bucket) value of put_object function.
5. Deploy the changes
6. To test this function add a new txt file to the input bucket
7. In the lambda page open cloudwatch in metrics tab and check for the logs to debug.
8. you will find the resultant file in the output bucket.
