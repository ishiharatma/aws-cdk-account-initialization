# aws-cdk-account-initialization

[日本語](README.ja.md) | English

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
cdk bootstrap --profile <project name>-<environment>-setupuser --termination-protection true -c env=<environment>

```sh
npm run cdk:deploy:all --env=<environment>
Or
cdk deploy -c env=<environment> --profile <project name>-<environment>-setupuser --version-reporting false --path-metadata false --asset-metadatafalsedeploy
```

## Terminate

```sh
npm run cdk:destory
or
cdk destroy -c env=<environment> --profile <project name>-<environment>-setupuser
```

## License

This project is released under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.
