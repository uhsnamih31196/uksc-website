# managed-identity

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\managed-identity:<version>' = {
  name: 'exampleInstance'
  params: {
    location: 'location'
    resourcePrefix: 'resourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `location` |  | string |  |
| `resourcePrefix` |  | string |  |

## Resources

- [Microsoft.ManagedIdentity/userAssignedIdentities@2018-11-30](https://learn.microsoft.com/en-us/azure/templates/microsoft.managedidentity/2018-11-30/userassignedidentities)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `id` | string |  |
| `principalId` | string |  |
| `clientId` | string |  |