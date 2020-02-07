# cf-simple-ad

## 概要

- Simple AD、および管理用Windowsサーバーを作成するCloudFormationテンプレート

## 必要パラメータ

- 配置対象のVPC
- 利用ドメイン名
- 配置対象のSubnet(Simple AD向け)
- 配置対象のSubnet(管理用Windowsサーバー向け)
- Windowsサーバーで利用されるKey Pair
- Windowsサーバーで利用されるセキュリティグループ
- WindowsサーバーのSSMで利用されるS3バケット

## 作成されるAWSリソース

- Simple AD
- EC2
