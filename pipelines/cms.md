# cms

## Usage

```bicep
module exampleInstance 'ts/IacModules:\pipelines\cms:<version>' = {
  name: 'exampleInstance'
  params: {
    acrUseManagedIdentityCreds: acrUseManagedIdentityCreds
    alwaysOn: alwaysOn
    appServicePlanId: 'appServicePlanId'
    branchName: 'branchName'
    cmsContainerImage: 'cmsContainerImage'
    databaseName: 'databaseName'
    databasePassword: databasePassword
    databaseUser: 'databaseUser'
    detailedErrorLoggingEnabled: detailedErrorLoggingEnabled
    enabledForTemplateDeployment: 'enabledForTemplateDeployment'
    enablePurgeProtection: enablePurgeProtection
    enableRbacAuthorization: enableRbacAuthorization
    enableSoftDelete: 'enableSoftDelete'
    existingManagedIdentityCms: 'existingManagedIdentityCms'
    existingPrivateDnsZoneDb: 'existingPrivateDnsZoneDb'
    existingPrivateDnsZoneKeyvault: 'existingPrivateDnsZoneKeyvault'
    existingVnet: 'existingVnet'
    frontDoorId: 'frontDoorId'
    ftpsState: 'ftpsState'
    http20Enabled: http20Enabled
    httpLoggingEnabled: httpLoggingEnabled
    httpsOnly: httpsOnly
    kvSku: 'kvSku'
    kvSkuFamily: 'kvSkuFamily'
    location: 'location'
    persistentResourceGroup: 'persistentResourceGroup'
    publicNetworkAccess: 'publicNetworkAccess'
    requestTracingEnabled: requestTracingEnabled
    resourcePrefix: 'resourcePrefix'
    sqlDbSku: 'sqlDbSku'
    sqlDbTier: 'sqlDbTier'
    tenantId: 'tenantId'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `acrUseManagedIdentityCreds` | acrUseManagedIdentityCreds | bool |  |
| `alwaysOn` | alwaysOn | bool |  |
| `appServicePlanId` | Id of App service plan to use | string |  |
| `branchName` | The name of branch | string |  |
| `cmsContainerImage` | container image to use | string |  |
| `databaseName` | Name of database | string |  |
| `databasePassword` | password for SqlDB | error |  |
| `databaseUser` | database user for SqlDB | string |  |
| `detailedErrorLoggingEnabled` | detailedErrorLoggingEnabled | bool |  |
| `enabledForTemplateDeployment` | enabledForDeployment | string |  |
| `enablePurgeProtection` | enablePurgeProtection for KV | bool |  |
| `enableRbacAuthorization` | enable RbacAuthorization | bool |  |
| `enableSoftDelete` | enable SoftDelete | string |  |
| `existingManagedIdentityCms` | existingManagedIdentityCms | string |  |
| `existingPrivateDnsZoneDb` | existingPrivateDnsZoneDb | string |  |
| `existingPrivateDnsZoneKeyvault` | existingPrivateDnsZoneKeyvault | string |  |
| `existingVnet` | existingVnet | string |  |
| `frontDoorId` | Id of frontdoor | string |  |
| `ftpsState` | ftpsState | string |  |
| `http20Enabled` | http20Enabled | bool |  |
| `httpLoggingEnabled` | httpLoggingEnabled | bool |  |
| `httpsOnly` | httpsOnly | bool |  |
| `kvSku` | kvSku | string |  |
| `kvSkuFamily` | kvSkuFamily | string |  |
| `location` | The location of the resources. | string |  |
| `persistentResourceGroup` | The name of the resource group to deploy to. | string |  |
| `publicNetworkAccess` | publicNetworkAccess | string |  |
| `requestTracingEnabled` | requestTracingEnabled | bool |  |
| `resourcePrefix` | The prefix to use for all resources. | string |  |
| `sqlDbSku` | Sku for SqlDb | string |  |
| `sqlDbTier` | Tier for SqlDB | string |  |
| `tenantId` | The tenant ID of the Azure AD tenant used for authentication. | string |  |

## Referenced Resources

| Provider | Name | Scope |
| --- | --- | --- |
| Microsoft.Network/virtualNetworks@2019-11-01 | `existingVnet` | `resourceGroup(persistentResourceGroup)` |
| Microsoft.Network/privateDnsZones@2020-06-01 | `existingPrivateDnsZoneKeyvault` | `resourceGroup(persistentResourceGroup)` |
| Microsoft.Network/privateDnsZones@2020-06-01 | `existingPrivateDnsZoneDb` | `resourceGroup(persistentResourceGroup)` |
| Microsoft.ManagedIdentity/userAssignedIdentities@2018-11-30 | `existingManagedIdentityCms` | `resourceGroup(persistentResourceGroup)` |
| Microsoft.KeyVault/vaults@2022-07-01 | `keyVaultCms.outputs.name` | - |

## Resources

- [Microsoft.Network/virtualNetworks@2019-11-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2019-11-01/virtualnetworks)
- [Microsoft.Network/privateDnsZones@2020-06-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2020-06-01/privatednszones)
- [Microsoft.ManagedIdentity/userAssignedIdentities@2018-11-30](https://learn.microsoft.com/en-us/azure/templates/microsoft.managedidentity/2018-11-30/userassignedidentities)
- [Microsoft.KeyVault/vaults@2022-07-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.keyvault/2022-07-01/vaults)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `cmsHostName` | string |  |