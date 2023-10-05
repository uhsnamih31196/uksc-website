# email-communication-service

## Usage

```bicep
module exampleInstance 'ts/IacModules:\modules\email-communication-service:<version>' = {
  name: 'exampleInstance'
  params: {
    communicationServiceName: 'uksc-communication-service-dev'
    customDomainName: ''
    dataLocation: 'UK'
    emailServiceName: 'uksc-email-service-dev'
    location: 'global'
    senderUserName: 'DoNotReply'
}
}
```

## Parameters

| Parameter | Description | Type | Default |
| --- | --- | --- | --- |
| `communicationServiceName` | The resource name for communication service

- Character limit: 1-63
- Valid characters: Alphanumerics and hyphens.
- Can't start or end with hyphen.
- Can't use underscores.
- Resource name must be unique across Azure.
  | string | 'uksc-communication-service-dev' |
  | `customDomainName` | The custom domain name to be used with email communication service.
  This will only be used in staging and prod environments.
  For all other environments we will be using Azure Managed domain
  | string | '' |
  | `dataLocation` | The location where the email service stores its data at rest | string | 'UK' |
  | `emailServiceName` | The resource name for email communication service | string | 'uksc-email-service-dev' |
  | `location` | The geo-location where the resource lives | string | 'global' |
  | `senderUserName` | A sender username to be used when sending emails | string | 'DoNotReply' |

## Resources

- [Microsoft.Communication/emailServices@2023-04-01-preview](https://learn.microsoft.com/en-us/azure/templates/microsoft.communication/2023-04-01-preview/emailservices)
- [Microsoft.Communication/emailServices/domains@2023-03-31](https://learn.microsoft.com/en-us/azure/templates/microsoft.communication/2023-03-31/emailservices/domains)
- [Microsoft.Communication/emailServices/domains/senderUsernames@2023-03-31](https://learn.microsoft.com/en-us/azure/templates/microsoft.communication/2023-03-31/emailservices/domains/senderusernames)
- [Microsoft.Communication/communicationServices@2023-03-31](https://learn.microsoft.com/en-us/azure/templates/microsoft.communication/2023-03-31/communicationservices)