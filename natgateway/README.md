# cf-natgateway

## 概要

* NatGatewayを作成して、PrivateSubnetからInternetアクセスできるようにするCloudFormation

## 必要パラメータ

* NatGatewayを配置するPublic Subnet
* Private Subnetで利用しているRouting Table

## 作成されるAWSリソース

* NatGatewayで利用されるElasticIP
* NatGateway
* NatGatewayを利用するRoutingTableのRoute
