# 03 — AWS Automation with boto3

## Install
```bash
pip install boto3
```

On EC2 prefer IAM Role instead of hardcoded access keys.

## S3 Client
```python
import boto3

s3 = boto3.client("s3")
response = s3.list_buckets()

for bucket in response.get("Buckets", []):
    print(bucket["Name"])
```

## Upload File
```python
s3.upload_file("report.csv", "my-bucket", "reports/report.csv")
```

## Download File
```python
s3.download_file("my-bucket", "reports/report.csv", "report.csv")
```

## Handle Errors
```python
from botocore.exceptions import BotoCoreError, ClientError

try:
    s3.list_buckets()
except (BotoCoreError, ClientError) as exc:
    print(f"AWS error: {exc}")
```

## Company Thinking
- IAM least privilege
- region/config externalize
- retries/timeouts where relevant
- log resource identifiers, never secrets
- test wrappers instead of mixing boto3 everywhere

## Practice
Build function `upload_report(local_path, bucket, key)` with logging and exception handling.
