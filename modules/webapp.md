# webapp

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\webapp:<version>' = {
  name: 'exampleInstance'
  params: {
    acrUseManagedIdentityCreds: acrUseManagedIdentityCreds
    alwaysOn: alwaysOn
    appContainerImage: 'appContainerImage'
    appServicePlanId: 'appServicePlanId'
    appSettings: appSettings
    detailedErrorLoggingEnabled: detailedErrorLoggingEnabled
    frontDoorId: 'frontDoorId'
    ftpsState: 'ftpsState'
    http20Enabled: http20Enabled
    httpLoggingEnabled: httpLoggingEnabled
    httpsOnly: httpsOnly
    location: 'location'
    managedIdentityClientId: 'managedIdentityClientId'
    managedIdentityId: 'managedIdentityId'
    requestTracingEnabled: requestTracingEnabled
    resourcePrefix: 'resourcePrefix'
    vnetIntegrationSubnetId: 'vnetIntegrationSubnetId'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `acrUseManagedIdentityCreds` | acrUseManagedIdentityCreds | bool |  |
| `alwaysOn` | alwaysOn | bool |  |
| `appContainerImage` | container image to use in app | string |  |
| `appServicePlanId` | Id of App service plan to use | string |  |
| `appSettings` | appSettings | object (secure) |  |
| `detailedErrorLoggingEnabled` | detailedErrorLoggingEnabled | bool |  |
| `frontDoorId` | Id of frontdoor | string |  |
| `ftpsState` | ftpsState | string |  |
| `http20Enabled` | http20Enabled | bool |  |
| `httpLoggingEnabled` | httpLoggingEnabled | bool |  |
| `httpsOnly` | httpsOnly | bool |  |
| `location` | location | string |  |
| `managedIdentityClientId` | Client id of managed identity | string |  |
| `managedIdentityId` | Managed identity for authentication | string |  |
| `requestTracingEnabled` | requestTracingEnabled | bool |  |
| `resourcePrefix` | resourcePrefix | string |  |
| `vnetIntegrationSubnetId` | Subnet id for vnet integration | string |  |

## Resources

- [Microsoft.Web/sites@2021-02-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.web/2021-02-01/sites)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `appUrl` | string |  |