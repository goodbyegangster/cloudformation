# cf-alb-for-ecs-blue-green

## 概要

- ECSコンテナのBlue/Greenデプロイを実施する場合に必要となるALB一式

## 必要パラメータ

- ALBの名前
- ALB配置先VPC
- ALB配置先サブネット
- ALBで利用されるセキュリティグループ

## 作成されるAWSリソース

- ALB
- 80/TCPのリスナー
- 80/TCPのリスナーで利用されるターゲットグループ
- 8080/TCPのリスナー
- 8080/TCPのリスナーで利用されるターゲットグループ
