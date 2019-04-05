# cf-ecs-datadog-agent

## 概要

* AWS ECSから監視対象となる情報を取得する、Datadog Agent Containerを起動させるCloudFormation
* 収集する情報
  * Metric Collection
  * Process Collection
* Datadog公式マニュアル
  * https://docs.datadoghq.com/integrations/amazon_ecs/?tab=python

## 必要パラメータ

* Datadog API Key
* 対象となるECS Cluseter名

## 作成されるAWSリソース

* ECS Execution用IAM Role
* ECS Task用IAM Role
* ECS Task Difinition
* ECS Service Difinition
