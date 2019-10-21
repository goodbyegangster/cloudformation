# cf-waf-for-wafcharm

## 概要

* WafCharmを利用しているAWS WAFのログを、WafCharmに連携するテンプレート
  * 
* AWS WAFをアタッチ先はALB

## 必要パラメータ

* AWS WAF名
* AWS WAFのメトリックス名
* AWS WAFをアタッチするALBのARN
* Kinesis FirehoseのDelivery Stream名
* Lambdaのソースコードを配置するS3Bucket
* Lambdaのソースコードを配置するKey

## 作成されるAWSリソース

* AWS WAF
* S3 Bucket
* Kinesis Firehose用IAM Role
* Kinesis Firehose
* Lambda用IAM Role
* Lambda Function
