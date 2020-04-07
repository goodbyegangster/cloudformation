# cf-datasync-agent

## 概要

- DataSync Agentを作成するテンプレート
- DataSyncサービスポイント用VPCエンドポイントを作成するテンプレート

## 必要パラメータ

- DataSync AgentとVPCエンドポイントを配置するVPC ID
- DataSync AgentとVPCエンドポイントを配置するサブネットID
- DataSyncで利用するAMI
- DataSyncで利用するインスタンスタイプ
- DataSyncで利用するKey Pair
- DataSyncのEC2で利用するSSM用S3バケット
- DataSyncにアクセス可能となるネットワークCIDR(配置先VPCのCIDR)

## 利用AMI確認用コマンド

```sh
$ aws ssm get-parameter --name /aws/service/datasync/ami --region ap-northeast-1
```

## 作成されるAWSリソース

- DataSync Agent用IAM Role
- DataSync Agent用Instance Profile
- DataSync AgentとなるEC2インスタンス
- DataSync AgentとなるEC2インスタンスにアタッチされるセキュリティグループ
- DataSyncサービスポイント用VPCエンドポイント
- DataSyncサービスポイント用VPCエンドポイントにアタッチされるセキュリティグループ
