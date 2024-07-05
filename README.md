# aws-cdk-account-initialization

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
cdk bootstrap --profile elpit-<環境変数名>-setupuser --termination-protection true -c env=<環境変数名>

```sh
npm run cdk:deploy:all --env=<環境変数名>
Or
cdk deploy -c env=<環境変数名> --profile elpit-<環境変数名>-setupuser --version-reporting false --path-metadata false --asset-metadatafalsedeploy
```

## Terminate

```sh
npm run cdk:destory
or
cdk destroy -c env=<環境変数名> --profile elpit-<環境変数名>-setupuser
```
