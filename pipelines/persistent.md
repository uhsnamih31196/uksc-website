# persistent

## Usage

```bicep
module exampleInstance 'ts/IacModules:\pipelines\persistent:<version>' = {
  name: 'exampleInstance'
  params: {
    appServicesVnetIntegrationSubnetName: 'appServicesVnetIntegrationSubnetName'
    appServicesVnetIntegrationSubnetPrefix: 'appServicesVnetIntegrationSubnetPrefix'
    dbPrivateEndpointsSubnetName: 'dbPrivateEndpointsSubnetName'
    dbPrivateEndpointsSubnetPrefix: 'dbPrivateEndpointsSubnetPrefix'
    dnsZoneDbName: 'dnsZoneDbName'
    dnsZoneKvName: 'dnsZoneKvName'
    kvPrivateEndpointsSubnetName: 'kvPrivateEndpointsSubnetName'
    kvPrivateEndpointsSubnetPrefix: 'kvPrivateEndpointsSubnetPrefix'
    location: resourceGroup().location
    resourcePrefixCms: 'resourcePrefixCms'
    resourcePrefixWebsite: 'resourcePrefixWebsite'
    sharedServicesResourceGroup: 'shared-services'
    virtualNetworkAddressPrefix: 'virtualNetworkAddressPrefix'
    virtualNetworkName: 'virtualNetworkName'
    vnetName: 'vnetName'
    vnetresourcePrefix: 'vnetresourcePrefix'
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
| `dnsZoneDbName` | dnszone db name | string |  |
| `dnsZoneKvName` | dnszone keyvault name | string |  |
| `kvPrivateEndpointsSubnetName` | kv PrivateEndpoints SubnetName | string |  |
| `kvPrivateEndpointsSubnetPrefix` | kv PrivateEndpointsSubnetPrefix | string |  |
| `location` | location of the deployment | string | `resourceGroup().location` |
| `resourcePrefixCms` | resource prefix cms | string |  |
| `resourcePrefixWebsite` | resource prefix website | string |  |
| `sharedServicesResourceGroup` | name of the resource group for the shared services | string | 'shared-services' |
| `virtualNetworkAddressPrefix` | virtualNetwork AddressPrefix | string |  |
| `virtualNetworkName` | virtual Network Name | string |  |
| `vnetName` | name of the vnet | string |  |
| `vnetresourcePrefix` | vnet resource prefix | string |  |