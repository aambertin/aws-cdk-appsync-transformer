# API Reference

**Classes**

Name|Description
----|-----------
[AppSyncTransformer](#aws-cdk-appsync-transformer-appsynctransformer)|AppSyncTransformer Construct.


**Structs**

Name|Description
----|-----------
[AppSyncTransformerProps](#aws-cdk-appsync-transformer-appsynctransformerprops)|Properties for AppSyncTransformer Construct.



## class AppSyncTransformer 🔹 <a id="aws-cdk-appsync-transformer-appsynctransformer"></a>

AppSyncTransformer Construct.

__Implements__: [IConstruct](#constructs-iconstruct), [IConstruct](#aws-cdk-core-iconstruct), [IConstruct](#constructs-iconstruct), [IDependable](#aws-cdk-core-idependable)
__Extends__: [Construct](#aws-cdk-core-construct)

### Initializer




```ts
new AppSyncTransformer(scope: Construct, id: string, props: AppSyncTransformerProps)
```

* **scope** (<code>[Construct](#aws-cdk-core-construct)</code>)  *No description*
* **id** (<code>string</code>)  *No description*
* **props** (<code>[AppSyncTransformerProps](#aws-cdk-appsync-transformer-appsynctransformerprops)</code>)  *No description*
  * **schemaPath** (<code>string</code>)  Required. 
  * **apiName** (<code>string</code>)  Optional. __*Default*__: `${id}-api`
  * **authorizationConfig** (<code>[AuthorizationConfig](#aws-cdk-aws-appsync-authorizationconfig)</code>)  Optional. __*Default*__: API_KEY authorization config
  * **fieldLogLevel** (<code>[FieldLogLevel](#aws-cdk-aws-appsync-fieldloglevel)</code>)  Optional. __*Default*__: FieldLogLevel.NONE
  * **syncEnabled** (<code>boolean</code>)  Optional. __*Default*__: false



### Properties


Name | Type | Description 
-----|------|-------------
**appsyncAPI**🔹 | <code>[GraphQLApi](#aws-cdk-aws-appsync-graphqlapi)</code> | <span></span>
**nestedAppsyncStack**🔹 | <code>[NestedStack](#aws-cdk-core-nestedstack)</code> | <span></span>
**tableNameMap**🔹 | <code>any</code> | <span></span>



## struct AppSyncTransformerProps 🔹 <a id="aws-cdk-appsync-transformer-appsynctransformerprops"></a>


Properties for AppSyncTransformer Construct.



Name | Type | Description 
-----|------|-------------
**schemaPath**🔹 | <code>string</code> | Required.
**apiName**?🔹 | <code>string</code> | Optional.<br/>__*Default*__: `${id}-api`
**authorizationConfig**?🔹 | <code>[AuthorizationConfig](#aws-cdk-aws-appsync-authorizationconfig)</code> | Optional.<br/>__*Default*__: API_KEY authorization config
**fieldLogLevel**?🔹 | <code>[FieldLogLevel](#aws-cdk-aws-appsync-fieldloglevel)</code> | Optional.<br/>__*Default*__: FieldLogLevel.NONE
**syncEnabled**?🔹 | <code>boolean</code> | Optional.<br/>__*Default*__: false



