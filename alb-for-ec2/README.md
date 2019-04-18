# cf-alb-for-ec2

## 概要

* Internet向けの、EC2用ALBを作成するCloudFormation

## 必要パラメータ

* 配置対象のVPC
* 配置対象のSubnet
* ロードバランサー名
* アタッチされるEC2

## 作成されるAWSリソース

* Security Group
* S3 Bucket(ALB用ログ)
* Application Load Blancer
* TargetGrouop
