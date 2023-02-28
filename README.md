# CloudFormationのサンプル（SNS・SQS）

## スタック作成

```
$ aws cloudformation create-stack --stack-name <StackName> --template-body file://template.yaml
```

## SNS/SQS

```
$ aws sns publish --topic-arn <TopicArn> --message "Hello World!"

$ aws sqs receive-message --queue-url <QueueURL>
```

## スタック削除

```
$ aws cloudformation delete-stack --stack-name <StackName>
```
