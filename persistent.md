# persistent

## Usage

```bicep
module exampleInstance 'ts/IacModules:\persistent:<version>' = {
  name: 'exampleInstance'
  params: {
    acrName: 'acrName'
    appServicesVnetIntegrationSubnetName: 'appServicesVnetIntegrationSubnetName'
    appServicesVnetIntegrationSubnetPrefix: 'appServicesVnetIntegrationSubnetPrefix'
    communicationServiceName: 'communicationServiceName'
    dbPrivateEndpointsSubnetName: 'dbPrivateEndpointsSubnetName'
    dbPrivateEndpointsSubnetPrefix: 'dbPrivateEndpointsSubnetPrefix'
    dnsZoneDbName: 'dnsZoneDbName'
    dnsZoneKvName: 'dnsZoneKvName'
    kvPrivateEndpointsSubnetName: 'kvPrivateEndpointsSubnetName'
    kvPrivateEndpointsSubnetPrefix: 'kvPrivateEndpointsSubnetPrefix'
    location: resourceGroup().location
    resourcePrefixCms: 'resourcePrefixCms'
    resourcePrefixWebsite: 'resourcePrefixWebsite'
    sharedServicesResourceGroup: 'sharedServicesResourceGroup'
    virtualNetworkAddressPrefix: 'virtualNetworkAddressPrefix'
    virtualNetworkName: 'virtualNetworkName'
    vnetresourcePrefix: 'vnetresourcePrefix'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `acrName` | name of the acr | string |  |
| `appServicesVnetIntegrationSubnetName` | appServices VnetIntegration SubnetName | string |  |
| `appServicesVnetIntegrationSubnetPrefix` | appServices VnetIntegrationSubnetPrefix | string |  |
| `communicationServiceName` | existing name of cummunication service | string |  |
| `dbPrivateEndpointsSubnetName` | db PrivateEndpoints SubnetName | string |  |
| `dbPrivateEndpointsSubnetPrefix` | db PrivateEndpointsSubnetPrefix | string |  |
| `dnsZoneDbName` | dnszone db name | string |  |
| `dnsZoneKvName` | dnszone keyvault name | string |  |
| `kvPrivateEndpointsSubnetName` | kv PrivateEndpoints SubnetName | string |  |
| `kvPrivateEndpointsSubnetPrefix` | kv PrivateEndpointsSubnetPrefix | string |  |
| `location` | location of the deployment | string | `resourceGroup().location` |
| `resourcePrefixCms` | resource prefix cms | string |  |
| `resourcePrefixWebsite` | resource prefix website | string |  |
| `sharedServicesResourceGroup` | name of the resource group for the shared services | string |  |
| `virtualNetworkAddressPrefix` | virtualNetwork AddressPrefix | string |  |
| `virtualNetworkName` | virtual Network Name | string |  |
| `vnetresourcePrefix` | vnet resource prefix | string |  |