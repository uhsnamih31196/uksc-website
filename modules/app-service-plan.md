# app-service-plan

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\app-service-plan:<version>' = {
  name: 'exampleInstance'
  params: {
    aspKind: 'aspKind'
    aspSku: 'aspSku'
    aspTier: 'aspTier'
    location: 'location'
    resourcePrefix: 'resourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `aspKind` | Please update kind for App Service Plan it can be Windows or Linux | string |  |
| `aspSku` | Please update SKU for App Service Plan | string |  |
| `aspTier` | Please update Tier for App Service Plan | string |  |
| `location` | Please update the location for deployment of App Service Plan | string |  |
| `resourcePrefix` | Unique String | string |  |

## Resources

- [Microsoft.Web/serverfarms@2020-06-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.web/2020-06-01/serverfarms)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `id` | string |  |