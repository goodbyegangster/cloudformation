# cf-iam-user-for-ansible-ec2-dynamic-invetory

## 概要

* Ansibleの `EC2 external inventory script` で利用するIAMユーザを作成するCloudFormation
  * [Ansible - Inventory Script Example: AWS EC2](https://docs.ansible.com/ansible/latest/user_guide/intro_dynamic_inventory.html#inventory-script-example-aws-ec2)
* IAMポリシー `AmazonEC2ReadOnlyAccess` の付与

## 必要パラメータ

* なし

## 作成されるAWSリソース

* IAM Group
* IAM User
* Access Key