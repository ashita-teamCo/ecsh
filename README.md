# ecsh

## Prerequirements

- [AWS CLI がインストール](https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/getting-started-install.html) されていること
  - [設定](https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/cli-configure-quickstart.html) が完了していること
- [Session Manager プラグインがインストール](https://docs.aws.amazon.com/ja_jp/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html) されていること

## Usage

`ecsh` を適当な場所に配置して PATH を通しておきます。

詳細は [ブログ記事「サッと ECS Exec でシェルを起動したいときに使えるスクリプト」](https://engineer.ashita-team.com/entry/introducing-a-wrapper-script-to-use-ecs-exec-more-easily) を参照してください。

```bash
$ ecsh
Usage: ecsh (OPTION cluster|profile) [OPTION service|container|region] ...
-C, --cluster:   Part of the cluster name (REQUIRED)
-s, --service:   Service name (default 'app')
-c, --container: Container name (default 'app')
-p, --profile:   AWS profile name (use environment variable 'AWS_PROFILE' as the default value)
-r, --region:    AWS region name (default 'ap-northeast-1')
```
