https://docs.aws.amazon.com/managedservices/latest/userguide/custom-cloudwatch-events.html

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/monitoring-scripts-intro.html

Cloudformation tamplete with create EC2 instance, security group with open port 80&443, and Instance policy which attach it to EC2. IAM Role allow the instance push logs to CloudWatch.
User Data of EC2 contains simple apache website and custom metrics like MemoryUsage, MemoryAvailable, and MemoryUtilization which are sending every 5 minutes to CloudWatch.