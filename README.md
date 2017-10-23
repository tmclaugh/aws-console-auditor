# aws-console-auditor

Service to record and store AWS console logins.

![Architecture Diagram](serverless-aws-console-auditor.png)

This service records AWS console login events.  When a user logs in a CloudTrail event is created.  This will trigger a lambda function that will record the event to S3.  This provides a record of console logins that can be referenced later.
