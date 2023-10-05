# components

## Usage

```bicep
module exampleInstance 'ts/IacModules:\components:<version>' = {
  name: 'exampleInstance'
  params: {
    acrUseManagedIdentityCreds: acrUseManagedIdentityCreds
    alwaysOn: alwaysOn
    aspKind: 'aspKind'
    aspSku: 'aspSku'
    aspTier: 'aspTier'
    cmsContainerImage: 'cmsContainerImage'
    databaseName: 'databaseName'
    databasePassword: 'databasePassword'
    databaseUser: 'databaseUser'
    dbPrivateEndpointsSubnetName: 'dbPrivateEndpointsSubnetName'
    detailedErrorLoggingEnabled: detailedErrorLoggingEnabled
    enabledForTemplateDeployment: 'enabledForTemplateDeployment'
    enablePurgeProtection: enablePurgeProtection
    enableRbacAuthorization: enableRbacAuthorization
    enableSoftDelete: 'enableSoftDelete'
    existingManagedIdentityCms: 'existingManagedIdentityCms'
    existingManagedIdentitywebsite: 'existingManagedIdentitywebsite'
    existingPrivateDnsZoneDb: 'existingPrivateDnsZoneDb'
    existingPrivateDnsZoneKeyvault: 'existingPrivateDnsZoneKeyvault'
    existingVnet: 'existingVnet'
    frontDoorSku: 'frontDoorSku'
    ftpsState: 'ftpsState'
    http20Enabled: http20Enabled
    httpLoggingEnabled: httpLoggingEnabled
    httpsOnly: httpsOnly
    kvPrivateEndpointsSubnetName: 'kvPrivateEndpointsSubnetName'
    kvSku: 'kvSku'
    kvSkuFamily: 'kvSkuFamily'
    location: 'location'
    persistentResourceGroup: 'persistentResourceGroup'
    publicNetworkAccess: 'publicNetworkAccess'
    requestTracingEnabled: requestTracingEnabled
    resourcePrefix: 'uniqueString(resourceGroup().id)'
    sqlDbSku: 'sqlDbSku'
    sqlDbTier: 'sqlDbTier'
    tenantId: 'tenantId'
    websiteContainerImage: 'websiteContainerImage'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `acrUseManagedIdentityCreds` | acrUseManagedIdentityCreds | bool |  |
| `alwaysOn` | alwaysOn | bool |  |
| `aspKind` | Update kind for App Service Plan it can be Windows or Linux | string |  |
| `aspSku` | Update SKU for App Service Plan | string |  |
| `aspTier` | Update Tier for App Service Plan | string |  |
| `cmsContainerImage` | cmsContainerImage | string |  |
| `databaseName` | databaseName | string |  |
| `databasePassword` | databasePassword | string |  |
| `databaseUser` | databaseUser | string |  |
| `dbPrivateEndpointsSubnetName` | db PrivateEndpoints SubnetName | string |  |
| `detailedErrorLoggingEnabled` | detailedErrorLoggingEnabled | bool |  |
| `enabledForTemplateDeployment` | enableForTemplateDeployment | string |  |
| `enablePurgeProtection` | enablePurgeProtection for KV | bool |  |
| `enableRbacAuthorization` | enableRbacAuthorization | bool |  |
| `enableSoftDelete` | enableSoftDelete | string |  |
| `existingManagedIdentityCms` | existingManagedIdentityCms | string |  |
| `existingManagedIdentitywebsite` | managed identity for Website app | string |  |
| `existingPrivateDnsZoneDb` | existingPrivateDnsZoneDb | string |  |
| `existingPrivateDnsZoneKeyvault` | existingPrivateDnsZoneKeyvault | string |  |
| `existingVnet` | existingVnet | string |  |
| `frontDoorSku` | Update SKU for FrontDoor | string |  |
| `ftpsState` | ftpsState | string |  |
| `http20Enabled` | http20Enabled | bool |  |
| `httpLoggingEnabled` | httpLoggingEnabled | bool |  |
| `httpsOnly` | httpsOnly | bool |  |
| `kvPrivateEndpointsSubnetName` | kv PrivateEndpoints SubnetName | string |  |
| `kvSku` | kvSku | string |  |
| `kvSkuFamily` | kvSkuFamily | string |  |
| `location` | Location | string |  |
| `persistentResourceGroup` | persistentResourceGroup | string |  |
| `publicNetworkAccess` | publicNetworkAccess | string |  |
| `requestTracingEnabled` | requestTracingEnabled | bool |  |
| `resourcePrefix` | Resource prefix | string | uniqueString(resourceGroup().id) |
| `sqlDbSku` | sqlDbSku | string |  |
| `sqlDbTier` | sqlDbTier | string |  |
| `tenantId` | tenantId | string |  |
| `websiteContainerImage` | websiteContainerImage | string |  |