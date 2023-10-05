# private-dns

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\private-dns:<version>' = {
  name: 'exampleInstance'
  params: {
    dnsZoneName: 'dnsZoneName'
    virtualNetworkId: 'virtualNetworkId'
    virtualNetworkName: 'virtualNetworkName'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `dnsZoneName` |  | string |  |
| `virtualNetworkId` |  | string |  |
| `virtualNetworkName` |  | string |  |

## Resources

- [Microsoft.Network/privateDnsZones@2020-06-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2020-06-01/privatednszones)
- [Microsoft.Network/privateDnsZones/virtualNetworkLinks@2020-06-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2020-06-01/privatednszones/virtualnetworklinks)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `dnsZoneId` | string |  |
| `dnsZoneFqdn` | string |  |