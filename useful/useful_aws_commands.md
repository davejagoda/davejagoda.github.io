---
title: Useful AWS commands
layout: appleII
---

access keys
-----------
```
aws iam create-access-key

aws iam update-access-key

aws iam list-access-keys

aws iam get-access-key-last-used

aws iam delete-access-key
```

logs
----
```
aws logs describe-log-groups

aws logs describe-log-groups | grep logGroupName

aws logs describe-log-streams --log-group-name <LOG_GROUP_NAME>

aws logs describe-log-streams --log-group-name <LOG_GROUP_NAME> | grep logStreamName

aws logs get-log-events --log-group-name <LOG_GROUP_NAME> --log-stream-name <LOG_STREAM_NAME>

aws logs tail <LOG_GROUP_NAME> --follow

aws logs tail <LOG_GROUP_NAME> --since 5m
```

organizations
-------------
```
aws organizations list-accounts --output table

aws organizations list-accounts --output table --query 'Accounts[*].[Name,Id,Arn,JoinedMethod,JoinedTimestamp,Status]'

aws organizations list-accounts --output table --query 'Accounts[].{Id: Id, Who: Email, State: Status, How: JoinedMethod, When: JoinedTimestamp}'

aws organizations list-delegated-administrators --output table

aws account get-primary-email --account-id <AWS_ACCOUNT_ID>

aws account start-primary-email-update --account-id <AWS_ACCOUNT_ID> --primary-email <AWS_ROOT_EMAIL_ADDRESS>

aws account accept-primary-email-update --account-id <AWS_ACCOUNT_ID> --otp <OTP> --primary-email <AWS_ROOT_EMAIL_ADDRESS>
```

s3
--
```
aws s3 ls
```
