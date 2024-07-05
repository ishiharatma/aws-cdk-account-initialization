# aws-cdk-account-initialization

日本語 | [English](README.md)

![banner](banner.png)

Initial account setup with AWS CDK.

## Build

```sh
cd source
npm install -g aws-cdk
npm i
```

## Deploy

```sh
cd source
```

```sh
npm run cdk:bootstrap
Or
cdk bootstrap --profile <プロジェクト名>-<環境変数名>-setupuser --termination-protection true -c env=<環境変数名>

```sh
npm run cdk:deploy:all --env=<環境変数名>
Or
cdk deploy -c env=<環境変数名> --profile <プロジェクト名>-<環境変数名>-setupuser --version-reporting false --path-metadata false --asset-metadatafalsedeploy
```

## Terminate

```sh
npm run cdk:destory
or
cdk destroy -c env=<環境変数名> --profile <プロジェクト名>-<環境変数名>-setupuser
```

## License

This project is released under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.
