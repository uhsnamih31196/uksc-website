# communication-service-rbac

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\communication-service-rbac:<version>' = {
  name: 'exampleInstance'
  params: {
    communicationServiceName: 'communicationServiceName'
    contributorBuiltInRoleId: 'b24988ac-6180-42a0-ab88-20f7382dd24c'
    principalId: 'principalId'
    resourcePrefix: 'resourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `communicationServiceName` | The resource name of azure communication service
| string |  |
| `contributorBuiltInRoleId` | This is the built-in contributor role.
See https://learn.microsoft.com/en-gb/azure/role-based-access-control/built-in-roles#contributor
| string | 'b24988ac-6180-42a0-ab88-20f7382dd24c' |
| `principalId` | Principal Id for assigning role | string |  |
| `resourcePrefix` | Unique string | string |  |

## Referenced Resources

| Provider | Name | Scope |
| --- | --- | --- |
| Microsoft.Communication/communicationServices@2023-04-01-preview | `communicationServiceName` | - |

## Resources

- [Microsoft.Communication/communicationServices@2023-04-01-preview](https://learn.microsoft.com/en-us/azure/templates/microsoft.communication/2023-04-01-preview/communicationservices)
- [Microsoft.Authorization/roleAssignments@2022-04-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.authorization/2022-04-01/roleassignments)