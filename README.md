### AWS Lambda + S3 Events: Image Processing

This mini-project demonstrates how to build a serverless image processing pipeline using Amazon S3 and AWS Lambda:

1. **Provision two S3 buckets** — one for original uploads ("source") and one for processed outputs ("processed").
2. **Set up an IAM role and permissions**, granting Lambda access to read from the source bucket, write to the processed bucket, and log to CloudWatch.
3. **Deploy the Lambda function** with image processing logic (e.g., pixelation), provided via a `.zip` deployment package.
4. **Configure an S3 trigger** on the source bucket to invoke the Lambda upon new object uploads.
5. **Test it out** by uploading an image — the function processes it and saves the result in the processed bucket.
