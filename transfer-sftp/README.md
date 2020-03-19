# cf-transfer-sftp.yml

## 概要

- AWS Transfer for SFTPを作成するためのCloudFormationテンプレート

## 事前準備

SFTPで利用する公開鍵を作成

```sh
$ mkdir ./ssh-key; ssh-keygen -t rsa -b 4096 -C "zunchan@example.com" -f ./ssh-key/id_rsa
```

## 必要パラメータ

- 利用するSFTPユーザー名
- 上記で作成した公開鍵

## 作成されるAWSリソース

- CloudwatchLogsアクセス用のIAM Role
- S3バケットアクセス用のユーザー共通となるIAM Role
- S3バケット
- SFTP Server
- SFTP User
