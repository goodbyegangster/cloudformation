# cf-ecs-container-instance

## 概要

* ECS Container Instance を作成するCloudFormation
* 作成されるInstance数は2台
* UserDataで以下の処理を実行
  * 以下パッケージをインストール
    * aws cli
    * wget
  * タイムゾーンをTokyo時間に変更
  * Cloudwatch Agentをインストール
    * 設定パラメータを、SSM Paramter Storeより取得
  * SSM Agentをインストール

## 必要パラメータ

* ECS Cluster Name
* ECS Container Instance の EC2 で利用する AMI ID
* ECS Container Instance の EC2 Instance Type
* ECS Container Instance の EC2 で利用する Key Pair
* ECS Container Instance に アタッチする Security Group
* ECS Container Instance を配置する Subnet
* Cloudwatch Agent で参照される SSM Paramter Store名

## 作成されるAWSリソース

* ECS Container Instance で利用されるIAM Role
* ECS Container Instance の Launch Configuration
* ECS Container Instance の AutoScaling Group

