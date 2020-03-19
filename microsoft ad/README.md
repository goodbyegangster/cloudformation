# cf-microsoft-ad.yml

## 概要

- Microsoft AD、および管理用Windowsサーバーを作成するCloudFormationテンプレート

## 必要パラメータ

- MS AD配置先のVPC、サブネット
- MS ADで利用するドメイン名
- MS ADで利用するEdition
- 管理用Windowsサーバーの配置先Subnet
- Windowsサーバーで利用されるKey Pair
- Windowsサーバーで利用されるセキュリティグループ
- WindowsサーバーのSSMで利用されるS3バケット

## 作成されるAWSリソース

- Microsoft AD
- Microsoft ADを操作用のWindowsサーバー(EC2)
