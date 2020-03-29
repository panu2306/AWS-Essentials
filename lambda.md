# AWS Lambda

AWS Lambda is the serverless function-as-a-service offered by AWS. Now, by serverless we might think it is actually serverless but wait. It's nothing like that. By serveless we mean we do not need to manage the runtime environment or server for running particular function. Before some time, serverless is just limited to funtion-as-a-service. But now AWS offers Dynamodb, AWS Cognito, AWS API Gateway, Amazon S3 etc. services which are serverless i.e. their servers are managed by AWS. 

Now, coming back to AWS Lambda, the service is nothing but a small virtual function that runs as per our demand, scales automatically and we do not need t manage server unlike Amazon EC2. 

### Benifits: 
- Easy Pricing
- Integration with whole AWS stack 
- Supports many programming languages(Python, Javasript, Ruby, Scala, Go etc.)
- Easy to get more resources per function
- Easy to monitor using Cloudwatch. 

### Pricing:
AWS lambda is cheaper service, you can check the pricing details of AWS lambda [here](https://aws.amazon.com/lambda/pricing/).

### AWS Lambda Concurrancy & Throttling: 
Concurrency plays an important role in reference with performance. AWS can run 1000 executions/functions at a time by default. Each invocation over the concurrency limit will trigger a "Throttle". Throttle behavior will trigger on two invocations: if it is a synchronous invocation it will return ThrottleError-499 and if it is asynchronous invocation it will retry automatically and then goes to DLQ(Dead Letter Queue). 

### AWS Lambda Logging, Monitoring and Tracing: 
AWS Lambda execution logs are stored in AWS CloudWatch Logs and execution metrics are stored in AWS CloudWatch Metrics. Also, AWS X-Ray can be used for debugging and stack-tracing the lambda functions.  

### AWS Versions and Aliases: 
Aws Lambda captures its changes into varsions. By default user works in `$LATEST` version which is only mutable version. Other versions are immutable versions. Now, aliases are the pointers to different versions. Generally, different aliases are created for different environments like `PRODUCTION, DEV, TEST` etc. 



