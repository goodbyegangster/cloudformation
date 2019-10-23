# cf-glue-dev-endpoint

## 概要

* Glue Dev Endpointを作成するテンプレート

## 事前作業

* エンドポイントで利用するOpenSSHの鍵を作成しておく
* エンドポイント配置するSubnetには、S3エンドポイントまたはNAT Gatewayを配置しておく

## 事後作業

* エンドポイントにGrobalIPを付与する場合、Endpointで利用されるENIにEIPを付与する

## 必要パラメータ

* EndpointName
* VpcId
* SubnetId
* PublicKey(利用する公開鍵)

## 作成されるAWSリソース

* Glue用IAM Role
* Endpointで利用するSecurityGroup
* Glue Dev Endpoint
