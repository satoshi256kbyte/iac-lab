# 個人的なIaCのサンプル集です

## IaCを書くときに便利なTips

RDSの選択できるEngineVersionを取得するコマンド

Aurora MySQLの場合

```shell
aws rds describe-db-engine-versions --engine aurora-mysql --query 'DBEngineVersions[].EngineVersion'
```

Aurora PostgreSQLの場合

```shell
aws rds describe-db-engine-versions --engine aurora-postgresql --query 'DBEngineVersions[].EngineVersion'
```

CloudFormationのパラメータにおける、AWS固有のパラメータタイプ

https://docs.aws.amazon.com/ja_jp/AWSCloudFormation/latest/UserGuide/cloudformation-supplied-parameter-types.html


