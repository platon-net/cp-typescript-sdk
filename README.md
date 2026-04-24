## cp-typescript-sdk@1.0.0

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install cp-typescript-sdk@1.0.0 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *https://setup.platon.sk/api*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DNSApi* | [**createDnsRecord**](docs/DNSApi.md#creatednsrecord) | **POST** /dns/{domain}/records | Create DNS record
*DNSApi* | [**deleteDnsRecord**](docs/DNSApi.md#deletednsrecord) | **DELETE** /dns/{domain}/records/{recordId} | Delete DNS record
*DNSApi* | [**getDnsRecords**](docs/DNSApi.md#getdnsrecords) | **GET** /dns/{domain}/records | Get DNS records by domain
*DNSApi* | [**updateDnsRecord**](docs/DNSApi.md#updatednsrecord) | **PATCH** /dns/{domain}/records/{recordId} | Update DNS record
*DomainApi* | [**changeDomainNameservers**](docs/DomainApi.md#changedomainnameservers) | **PATCH** /domains/{domain}/nameservers | Change domain nameservers
*DomainApi* | [**closeDomain**](docs/DomainApi.md#closedomain) | **DELETE** /domains/{domain} | Close external customer domain product
*DomainApi* | [**getDomainInfo**](docs/DomainApi.md#getdomaininfo) | **GET** /domains/{domain} | Get domain information and availability
*DomainApi* | [**listDomains**](docs/DomainApi.md#listdomains) | **GET** /domains | List customer domains
*DomainApi* | [**registerDomain**](docs/DomainApi.md#registerdomain) | **POST** /domains/{domain}/register | Register domain
*DomainApi* | [**renewDomain**](docs/DomainApi.md#renewdomain) | **POST** /domains/{domain}/renew | Renew domain
*EmailApi* | [**changeMailboxPassword**](docs/EmailApi.md#changemailboxpassword) | **PATCH** /email/{domain}/mailboxes/{username}/password | Change mailbox password
*EmailApi* | [**createMailbox**](docs/EmailApi.md#createmailbox) | **POST** /email/{domain}/mailboxes | Create mailbox
*OAuthApi* | [**createOauthRequest**](docs/OAuthApi.md#createoauthrequest) | **POST** /oauth/requests | Create OAuth request
*OAuthApi* | [**deleteOauthToken**](docs/OAuthApi.md#deleteoauthtoken) | **DELETE** /oauth/tokens | Delete OAuth token
*OAuthApi* | [**getOauthScopes**](docs/OAuthApi.md#getoauthscopes) | **GET** /oauth/scopes | List available OAuth scopes
*OAuthApi* | [**refreshOauthToken**](docs/OAuthApi.md#refreshoauthtoken) | **POST** /oauth/tokens/refresh | Refresh OAuth token
*OAuthApi* | [**verifyOauthRequest**](docs/OAuthApi.md#verifyoauthrequest) | **GET** /oauth/requests/verify | Verify OAuth request
*SystemApi* | [**hello**](docs/SystemApi.md#hello) | **GET** /system/hello | Returns greeting message
*SystemApi* | [**revision**](docs/SystemApi.md#revision) | **GET** /system/revision | Returns revision number of system
*SystemApi* | [**time**](docs/SystemApi.md#time) | **GET** /system/time | Returns current date and time of system
*VehicleApi* | [**createVehicleEvent**](docs/VehicleApi.md#createvehicleevent) | **POST** /vehicle/events | Create vehicle event without receipt image
*VehicleApi* | [**deleteVehicleEvent**](docs/VehicleApi.md#deletevehicleevent) | **DELETE** /vehicle/events/{eventId} | Delete vehicle event
*VehicleApi* | [**finalizeVehicleEvent**](docs/VehicleApi.md#finalizevehicleevent) | **POST** /vehicle/events/{eventId}/finalize | Finalize vehicle event draft
*VehicleApi* | [**getVehicleEvent**](docs/VehicleApi.md#getvehicleevent) | **GET** /vehicle/events/{eventId} | Get vehicle event detail
*VehicleApi* | [**getVehicleEventImage**](docs/VehicleApi.md#getvehicleeventimage) | **GET** /vehicle/events/{eventId}/image | Get event image or thumbnail
*VehicleApi* | [**listVehicleCurrencies**](docs/VehicleApi.md#listvehiclecurrencies) | **GET** /vehicle/currencies | List currencies for vehicle events
*VehicleApi* | [**listVehicleEvents**](docs/VehicleApi.md#listvehicleevents) | **GET** /vehicle/events | List vehicle events for the authenticated driver
*VehicleApi* | [**listVehicleVehicles**](docs/VehicleApi.md#listvehiclevehicles) | **GET** /vehicle/vehicles | List vehicles available to the authenticated driver
*VehicleApi* | [**rescanVehicleEventImage**](docs/VehicleApi.md#rescanvehicleeventimage) | **POST** /vehicle/events/{eventId}/image | Replace event image and rescan event data
*VehicleApi* | [**setPreferredVehicle**](docs/VehicleApi.md#setpreferredvehicle) | **PATCH** /vehicle/preferred-vehicle | Set or clear preferred vehicle
*VehicleApi* | [**uploadVehicleReceiptImage**](docs/VehicleApi.md#uploadvehiclereceiptimage) | **POST** /vehicle/events/receipt-image | Upload receipt image and create processing event draft


### Documentation For Models

 - [ChangeDomainNameserversRequest](docs/ChangeDomainNameserversRequest.md)
 - [ChangeMailboxPasswordRequest](docs/ChangeMailboxPasswordRequest.md)
 - [CreateDnsRecord200Response](docs/CreateDnsRecord200Response.md)
 - [CreateDnsRecordRequest](docs/CreateDnsRecordRequest.md)
 - [CreateMailboxRequest](docs/CreateMailboxRequest.md)
 - [CreateOauthRequest200Response](docs/CreateOauthRequest200Response.md)
 - [CreateOauthRequest200ResponseData](docs/CreateOauthRequest200ResponseData.md)
 - [CreateOauthRequestRequest](docs/CreateOauthRequestRequest.md)
 - [CreateVehicleEventRequest](docs/CreateVehicleEventRequest.md)
 - [DeleteOauthToken200Response](docs/DeleteOauthToken200Response.md)
 - [DeleteOauthToken200ResponseData](docs/DeleteOauthToken200ResponseData.md)
 - [FinalizeVehicleEventRequest](docs/FinalizeVehicleEventRequest.md)
 - [FinalizeVehicleEventRequestFueling](docs/FinalizeVehicleEventRequestFueling.md)
 - [FinalizeVehicleEventRequestLocation](docs/FinalizeVehicleEventRequestLocation.md)
 - [FinalizeVehicleEventRequestMoney](docs/FinalizeVehicleEventRequestMoney.md)
 - [GetDnsRecords200Response](docs/GetDnsRecords200Response.md)
 - [GetDnsRecords200ResponseData](docs/GetDnsRecords200ResponseData.md)
 - [GetDnsRecords200ResponseDataRecordsInner](docs/GetDnsRecords200ResponseDataRecordsInner.md)
 - [GetOauthScopes200Response](docs/GetOauthScopes200Response.md)
 - [GetOauthScopes200ResponseDataInner](docs/GetOauthScopes200ResponseDataInner.md)
 - [Hello200Response](docs/Hello200Response.md)
 - [Hello200ResponseData](docs/Hello200ResponseData.md)
 - [ListDomains200Response](docs/ListDomains200Response.md)
 - [ListDomains200ResponseData](docs/ListDomains200ResponseData.md)
 - [RefreshOauthTokenRequest](docs/RefreshOauthTokenRequest.md)
 - [RegisterDomainRequest](docs/RegisterDomainRequest.md)
 - [RenewDomainRequest](docs/RenewDomainRequest.md)
 - [Revision200Response](docs/Revision200Response.md)
 - [Revision200ResponseData](docs/Revision200ResponseData.md)
 - [SetPreferredVehicleRequest](docs/SetPreferredVehicleRequest.md)
 - [Time200Response](docs/Time200Response.md)
 - [Time200ResponseData](docs/Time200ResponseData.md)
 - [UpdateDnsRecordRequest](docs/UpdateDnsRecordRequest.md)
 - [VerifyOauthRequest200Response](docs/VerifyOauthRequest200Response.md)
 - [VerifyOauthRequest200ResponseData](docs/VerifyOauthRequest200ResponseData.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="bearerAuth"></a>
### bearerAuth

- **Type**: Bearer authentication

