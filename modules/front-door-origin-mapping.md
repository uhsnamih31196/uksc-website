# front-door-origin-mapping

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\front-door-origin-mapping:<version>' = {
  name: 'exampleInstance'
  params: {
    frontDoorResourceName: 'frontDoorResourceName'
    hostName: 'hostName'
    patternsToMatch: patternsToMatch
    resourcePrefix: 'resourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `frontDoorResourceName` |  | string |  |
| `hostName` |  | string |  |
| `patternsToMatch` |  | array |  |
| `resourcePrefix` |  | string |  |

## Referenced Resources

| Provider | Name | Scope |
| --- | --- | --- |
| Microsoft.Cdn/profiles@2023-05-01 | `frontDoorResourceName` | - |
| Microsoft.Cdn/profiles/afdEndpoints@2023-05-01 | `resourcePrefix` | - |

## Resources

- [Microsoft.Cdn/profiles@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles)
- [Microsoft.Cdn/profiles/afdEndpoints@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles/afdendpoints)
- [Microsoft.Cdn/profiles/originGroups@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles/origingroups)
- [Microsoft.Cdn/profiles/originGroups/origins@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles/origingroups/origins)
- [Microsoft.Cdn/profiles/afdEndpoints/routes@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles/afdendpoints/routes)