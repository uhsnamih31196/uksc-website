# uksc-website

## Usage

```bicep
module exampleInstance 'ts/IacModules:\pipelines\uksc-website:<version>' = {
  name: 'exampleInstance'
  params: {
    acrUseManagedIdentityCreds: acrUseManagedIdentityCreds
    alwaysOn: alwaysOn
    appServicePlanId: 'appServicePlanId'
    cmsHostName: 'cmsHostName'
    detailedErrorLoggingEnabled: detailedErrorLoggingEnabled
    enabledForTemplateDeployment: 'enabledForTemplateDeployment'
    enablePurgeProtection: enablePurgeProtection
    enableRbacAuthorization: enableRbacAuthorization
    enableSoftDelete: 'enableSoftDelete'
    frontDoorId: 'frontDoorId'
    ftpsState: 'ftpsState'
    http20Enabled: http20Enabled
    httpLoggingEnabled: httpLoggingEnabled
    httpsOnly: httpsOnly
    kvSku: 'kvSku'
    kvSkuFamily: 'kvSkuFamily'
    location: resourceGroup().location
    persistentResourceGroup: 'persistentResourceGroup'
    publicNetworkAccess: 'publicNetworkAccess'
    requestTracingEnabled: requestTracingEnabled
    resourcePrefix: 'uniqueString(resourceGroup().id)'
    tenantId: subscription().tenantId
    websiteContainerImage: 'websiteContainerImage'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `acrUseManagedIdentityCreds` | acrUseManagedIdentityCreds | bool |  |
| `alwaysOn` | alwaysOn | bool |  |
| `appServicePlanId` | appServicePlanId | string |  |
| `cmsHostName` | cmsHostName | string |  |
| `detailedErrorLoggingEnabled` | detailedErrorLoggingEnabled | bool |  |
| `enabledForTemplateDeployment` | enabledForDeployment | string |  |
| `enablePurgeProtection` | enablePurgeProtection for KV | bool |  |
| `enableRbacAuthorization` | enableRbacAuthorization | bool |  |
| `enableSoftDelete` | enableSoftDelete | string |  |
| `frontDoorId` | frontDoorId | string |  |
| `ftpsState` | ftpsState | string |  |
| `http20Enabled` | http20Enabled | bool |  |
| `httpLoggingEnabled` | httpLoggingEnabled | bool |  |
| `httpsOnly` | httpsOnly | bool |  |
| `kvSku` | kvSku | string |  |
| `kvSkuFamily` | kvSkuFamily | string |  |
| `location` | location | string | `resourceGroup().location` |
| `persistentResourceGroup` | persistentResourceGroup | string |  |
| `publicNetworkAccess` | publicNetworkAccess | string |  |
| `requestTracingEnabled` | requestTracingEnabled | bool |  |
| `resourcePrefix` | resourcePrefix | string | uniqueString(resourceGroup().id) |
| `tenantId` | tenantId | string | `subscription().tenantId` |
| `websiteContainerImage` | websiteContainerImage | string |  |

## Referenced Resources

| Provider | Name | Scope |
| --- | --- | --- |
| Microsoft.Network/virtualNetworks@2019-11-01 | `'vitrual-network'` | `resourceGroup(persistentResourceGroup)` |
| Microsoft.Network/privateDnsZones@2020-06-01 | `'privatelink.vaultcore.azure.net'` | `resourceGroup(persistentResourceGroup)` |
| Microsoft.ManagedIdentity/userAssignedIdentities@2018-11-30 | `'website-mi'` | `resourceGroup(persistentResourceGroup)` |

## Resources

- [Microsoft.Network/virtualNetworks@2019-11-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2019-11-01/virtualnetworks)
- [Microsoft.Network/privateDnsZones@2020-06-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2020-06-01/privatednszones)
- [Microsoft.ManagedIdentity/userAssignedIdentities@2018-11-30](https://learn.microsoft.com/en-us/azure/templates/microsoft.managedidentity/2018-11-30/userassignedidentities)