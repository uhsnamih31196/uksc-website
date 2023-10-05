# acr-pull-role-assignment

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\acr-pull-role-assignment:<version>' = {
  name: 'exampleInstance'
  params: {
    acrName: 'acrName'
    acrPullBuiltInRoleId: '7f951dda-4ed3-4680-a7ca-43fe172d538d'
    principalId: 'principalId'
    resourcePrefix: 'resourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `acrName` |  | string |  |
| `acrPullBuiltInRoleId` |  | string | '7f951dda-4ed3-4680-a7ca-43fe172d538d' |
| `principalId` |  | string |  |
| `resourcePrefix` |  | string |  |

## Referenced Resources

| Provider | Name | Scope |
| --- | --- | --- |
| Microsoft.ContainerRegistry/registries@2023-01-01-preview | `acrName` | - |

## Resources

- [Microsoft.ContainerRegistry/registries@2023-01-01-preview](https://learn.microsoft.com/en-us/azure/templates/microsoft.containerregistry/2023-01-01-preview/registries)
- [Microsoft.Authorization/roleAssignments@2022-04-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.authorization/2022-04-01/roleassignments)