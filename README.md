# AppSync Transformer Construct for AWS CDK

![build](https://github.com/kcwinner/aws-cdk-appsync-transformer/workflows/build/badge.svg)
[![codecov](https://codecov.io/gh/kcwinner/aws-cdk-appsync-transformer/branch/main/graph/badge.svg)](https://codecov.io/gh/kcwinner/aws-cdk-appsync-transformer)
[![dependencies Status](https://david-dm.org/kcwinner/aws-cdk-appsync-transformer/status.svg)](https://david-dm.org/kcwinner/aws-cdk-appsync-transformer)
[![npm](https://img.shields.io/npm/dt/aws-cdk-appsync-transformer)](https://www.npmjs.com/package/aws-cdk-appsync-transformer)

[![npm version](https://badge.fury.io/js/aws-cdk-appsync-transformer.svg)](https://badge.fury.io/js/aws-cdk-appsync-transformer)
[![NuGet version](https://badge.fury.io/nu/Kcwinner.AWSCDKAppSyncTransformer.svg)](https://badge.fury.io/nu/Kcwinner.AWSCDKAppSyncTransformer)
[![PyPI version](https://badge.fury.io/py/aws-cdk-appsync-transformer.svg)](https://badge.fury.io/py/aws-cdk-appsync-transformer)
[![Maven Central](https://img.shields.io/maven-central/v/io.github.kcwinner/AWSCDKAppSyncTransformer?color=brightgreen)](https://repo1.maven.org/maven2/io/github/kcwinner/AWSCDKAppSyncTransformer/)

## Why This Package

In April 2020 I wrote a [blog post](https://www.trek10.com/blog/appsync-with-the-aws-cloud-development-kit) on using the AWS Cloud Development Kit with AppSync. I wrote my own transformer in order to emulate AWS Amplify's method of using GraphQL directives in order to template a lot of the Schema Definition Language. 

This package is my attempt to convert all of that effort into a separate construct in order to clean up the process. 

## How Do I Use It

### Example TypeScript usage

```ts
import { AppSyncTransformer } from 'aws-cdk-appsync-transformer';
...
new AppSyncTransformer(this, "my-cool-api", {
    schemaPath: 'schema.graphql'
});
```

### [Supported Amplify Directives](https://docs.amplify.aws/cli/graphql-transformer/directives)

Tested:
* [@model](https://docs.amplify.aws/cli/graphql-transformer/directives#model)
* [@auth](https://docs.amplify.aws/cli/graphql-transformer/directives#auth)
* [@connection](https://docs.amplify.aws/cli/graphql-transformer/directives#connection)

Experimental:
* [@key](https://docs.amplify.aws/cli/graphql-transformer/directives#key)
* [@versioned](https://docs.amplify.aws/cli/graphql-transformer/directives#versioned)

Not Yet Supported:
* [@function](https://docs.amplify.aws/cli/graphql-transformer/directives#function)
* [@searchable](https://docs.amplify.aws/cli/graphql-transformer/directives#searchable)
* [@predictions](https://docs.amplify.aws/cli/graphql-transformer/directives#predictions)
* [@http](https://docs.amplify.aws/cli/graphql-transformer/directives#http)

### Code Generation

## Versioning

I will *attempt* to align the major and minor version of this package with [AWS CDK], but always check the release descriptions for compatibility.

I currently support [![GitHub package.json dependency version (prod)](https://img.shields.io/github/package-json/dependency-version/kcwinner/appsync-transformer-construct/@aws-cdk/core)](https://github.com/aws/aws-cdk)


[aws cdk]: https://aws.amazon.com/cdk