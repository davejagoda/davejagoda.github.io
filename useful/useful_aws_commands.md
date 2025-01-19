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
```

organizations
-------------
```
aws organizations list-accounts --output table

aws organizations list-delegated-administrators --output table
```

s3
--
```
aws s3 ls
```
