# cf-sns-and-kinesis-firehose

## 概要

- SESのNortification処理で利用される下記AWSリソースの作成
  - SNS
  - Kinesis Firehose
  - S3

## 必要パラメータ

- 利用するS3のバケット名 
- SESで設定するNortificationの種類

## 作成されるAWSリソース

- S3バケット
- Kinesis Firehose
- SNS Topic, Subscription
