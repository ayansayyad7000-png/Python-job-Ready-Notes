# AWS Automation with boto3

`boto3` is the AWS SDK for Python.

Install:
```bash
python -m pip install boto3
```

## List S3 Buckets
```python
import boto3

s3 = boto3.client("s3")
response = s3.list_buckets()

for bucket in response.get("Buckets", []):
    print(bucket["Name"])
```

## Upload a File
```python
s3.upload_file("report.txt", "my-bucket", "reports/report.txt")
```

## Credentials
Prefer IAM roles or workload identities. Do not hard-code access keys.

## Error Handling
```python
from botocore.exceptions import ClientError
```
Catch specific AWS errors when you can handle them meaningfully.

## Company Use
Cloud automation, platform tooling, resource inventory, deployment workflows, MLOps pipelines.

## Common Mistakes
- Hard-coded credentials
- Broad IAM permissions
- No pagination for large API results

## Interview Questions
1. What is boto3?
2. Why prefer IAM roles?
3. Why does pagination matter?