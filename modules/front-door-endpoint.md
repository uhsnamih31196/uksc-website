# front-door-endpoint

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\front-door-endpoint:<version>' = {
  name: 'exampleInstance'
  params: {
    frontDoorResourceName: 'frontDoorResourceName'
    resourcePrefix: 'resourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `frontDoorResourceName` |  | string |  |
| `resourcePrefix` |  | string |  |

## Referenced Resources

| Provider | Name | Scope |
| --- | --- | --- |
| Microsoft.Cdn/profiles@2023-05-01 | `frontDoorResourceName` | - |

## Resources

- [Microsoft.Cdn/profiles@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles)
- [Microsoft.Cdn/profiles/afdEndpoints@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles/afdendpoints)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `endpointHostName` | string |  |