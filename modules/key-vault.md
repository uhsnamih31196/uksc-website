# key-vault

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\key-vault:<version>' = {
  name: 'exampleInstance'
  params: {
    enabledForTemplateDeployment: 'enabledForTemplateDeployment'
    enablePurgeProtection: enablePurgeProtection
    enableRbacAuthorization: enableRbacAuthorization
    enableSoftDelete: 'enableSoftDelete'
    kvSku: 'kvSku'
    kvSkuFamily: 'kvSkuFamily'
    location: 'location'
    principalId: 'principalId'
    privateDnsZoneId: 'privateDnsZoneId'
    privateEndpointsSubnetId: 'privateEndpointsSubnetId'
    publicNetworkAccess: 'publicNetworkAccess'
    resourcePrefix: 'resourcePrefix'
    secretsObject: secretsObject
    tenantId: 'tenantId'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `enabledForTemplateDeployment` | Template deployment enablment for KV | string |  |
| `enablePurgeProtection` | enablePurgeProtection for KV | bool |  |
| `enableRbacAuthorization` | Enable Rbac Authorization for KV | bool |  |
| `enableSoftDelete` | Enable enableSoftDelete for KV | string |  |
| `kvSku` | kvsku for KV | string |  |
| `kvSkuFamily` | kvSkuFamily for KV | string |  |
| `location` | Please update the location for deployment of SQLDB | string |  |
| `principalId` | Principal ID for role assignment | string |  |
| `privateDnsZoneId` | PrivateDNSZone id | string |  |
| `privateEndpointsSubnetId` | Private Endpoint subnetid | string |  |
| `publicNetworkAccess` | Enable publicNetworkAccess for KV | string |  |
| `resourcePrefix` | resource prefix | string |  |
| `secretsObject` | Specifies all secrets {"name":"","value":""} wrapped in a secure object. | object (secure) |  |
| `tenantId` | Tenant ID | string |  |

## Resources

- [Microsoft.KeyVault/vaults@2023-02-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.keyvault/2023-02-01/vaults)
- [Microsoft.Network/privateEndpoints@2023-04-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2023-04-01/privateendpoints)
- [Microsoft.Network/privateEndpoints/privateDnsZoneGroups@2023-04-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2023-04-01/privateendpoints/privatednszonegroups)
- [Microsoft.Authorization/roleAssignments@2022-04-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.authorization/2022-04-01/roleassignments)
- [Microsoft.KeyVault/vaults/secrets@2021-04-01-preview](https://learn.microsoft.com/en-us/azure/templates/microsoft.keyvault/2021-04-01-preview/vaults/secrets)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `name` | string |  |