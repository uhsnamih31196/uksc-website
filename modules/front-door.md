# front-door

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\front-door:<version>' = {
  name: 'exampleInstance'
  params: {
    frontDoorSku: 'frontDoorSku'
    resourcePrefix: 'resourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `frontDoorSku` | SKU value for FrontDoor | string |  |
| `resourcePrefix` | Unique string | string |  |

## Resources

- [Microsoft.Cdn/profiles@2023-05-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.cdn/2023-05-01/profiles)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `id` | string |  |