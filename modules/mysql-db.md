# mysql-db

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\mysql-db:<version>' = {
  name: 'exampleInstance'
  params: {
    databaseName: '${resourcePrefix}-database'
    databasePassword: 'databasePassword'
    databaseUser: 'databaseUser'
    dnsZoneId: 'dnsZoneId'
    location: 'location'
    privateEndpointsSubnetId: 'privateEndpointsSubnetId'
    resourcePrefix: 'resourcePrefix'
    sqlDbSku: 'sqlDbSku'
    sqlDbTier: 'sqlDbTier'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `databaseName` | Database Name for SQLDB | string | `'${resourcePrefix}-database'` |
| `databasePassword` | Database Password for SQLDB | string (secure) |  |
| `databaseUser` | Database Password for SQLDB | string (secure) |  |
| `dnsZoneId` | Private DNS zone ID for SQLDB | string |  |
| `location` | Update the location for deployment of SQLDB | string |  |
| `privateEndpointsSubnetId` | Subnet ID of Private Endpoint for SQLDB | string |  |
| `resourcePrefix` | Unique String | string |  |
| `sqlDbSku` | Please update SKU for SqlDB | string |  |
| `sqlDbTier` | Please update Tier for SqlDB | string |  |

## Resources

- [Microsoft.DBforMySQL/flexibleServers/databases@2022-01-01](https://learn.microsoft.com/en-us/azure/templates/microsoft.dbformysql/2022-01-01/flexibleservers/databases)
- [Microsoft.DBforMySQL/flexibleServers@2022-09-30-preview](https://learn.microsoft.com/en-us/azure/templates/microsoft.dbformysql/2022-09-30-preview/flexibleservers)

## Outputs

| Name | Type | Description |
| --- | --- | --- |
| `databaseServerName` | string |  |
| `databaseName` | string |  |
| `databaseHostName` | string |  |