# cf-kinesisfirehose-for-s3-notransform

## 概要

* S3をDestinationとするKinesisFirehoseを作成
  * transformation処理はなし

## 必要パラメータ

* Delivery Stream名
* Destination先のS3バケット名
* Destination時のS3Prefix

## 作成されるAWSリソース

* IAM Role
* Kinesis FirehoseのDelivery Stream
