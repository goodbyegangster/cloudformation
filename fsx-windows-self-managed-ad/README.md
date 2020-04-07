# cf-FSx-windows-self-managed-ad

## 概要

- `FSx for Windows` をActiveDirectoryで利用するテンプレート
  - Single AZ

## 必要パラメータ

- `FSx for Windows` のENI配置先VPC
- `FSx for Windows` のENI配置先サブネット
- `FSx for Windows` のENIで利用するセキュリティグループ
- ActiveDirectoryのIPアドレス(参照先DNS)
- ActiveDirectoryのドメイン名
- ActiveDirectoryのOU名
- ActiveDirectoryのFSx用Adminグループ
- ActiveDirectoryのFSx用Adminユーザー
- FSx用Adminユーザーのパスワード
- `FSx for Windows` へアクセス元CIDR

## 作成されるAWSリソース

- FSx for Windows
- FSx for Windows用のセキュリティグループ
