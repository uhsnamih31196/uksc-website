# vnet

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\vnet:<version>' = {
  name: 'exampleInstance'
  params: {
    appServicesVnetIntegrationSubnetName: 'appServicesVnetIntegrationSubnetName'
    appServicesVnetIntegrationSubnetPrefix: 'appServicesVnetIntegrationSubnetPrefix'
    dbPrivateEndpointsSubnetName: 'dbPrivateEndpointsSubnetName'
    dbPrivateEndpointsSubnetPrefix: 'dbPrivateEndpointsSubnetPrefix'
    kvPrivateEndpointsSubnetName: 'kvPrivateEndpointsSubnetName'
    kvPrivateEndpointsSubnetPrefix: 'kvPrivateEndpointsSubnetPrefix'
    location: 'location'
    resourcePrefix: 'resourcePrefix'
    virtualNetworkAddressPrefix: 'virtualNetworkAddressPrefix'
    virtualNetworkName: 'virtualNetworkName'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `appServicesVnetIntegrationSubnetName` | appServices VnetIntegration SubnetName | string |  |
| `appServicesVnetIntegrationSubnetPrefix` | appServices VnetIntegrationSubnetPrefix | string |  |
| `dbPrivateEndpointsSubnetName` | db PrivateEndpoints SubnetName | string |  |
| `dbPrivateEndpointsSubnetPrefix` | db PrivateEndpointsSubnetPrefix | string |  |
| `kvPrivateEndpointsSubnetName` | kv PrivateEndpoints SubnetName | string |  |
| `kvPrivateEndpointsSubnetPrefix` | kv PrivateEndpointsSubnetPrefix | string |  |
| `location` | location | string |  |
| `resourcePrefix` | resourcePrefix for deployment of resources | string |  |
| `virtualNetworkAddressPrefix` | virtualNetwork AddressPrefix | string |  |
| `virtualNetworkName` | virtual Network Name | string |  |

## Resources

- [Microsoft.Network/networkSecurityGroups@2019-11-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2019-11-01/networksecuritygroups)
- [Microsoft.Network/virtualNetworks@2019-11-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.network/2019-11-01/virtualnetworks)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `virtualNetworkId` | string |  |
| `vnetIntegrationSubnetId` | string |  |
| `vnetIntegrationSubnetIpRange` | string |  |
| `dbPrivateEndpointsSubnetId` | string |  |
| `kvPrivateEndpointsSubnetId` | string |  |