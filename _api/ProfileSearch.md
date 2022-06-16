---
layout: post
---

﻿# ProfileSearch


Referenced Table: [profile](/profile)

| Column | Type | Size | Flags | Table | Description |
| ------ | ---- | ---- | ----- | ----- | ----------- |
| recNo | long |  | profile | 
| tagValue | string | 1024 | profile | 
| summaryCount | int |  | profile | 
| name | string | 256 | profile | 
| profileType | short |  | profile | 
| clientType | short |  | clientProfile | 
| supplierType | short |  | supplierProfile | 
| primaryPersonRecNo | long |  | profile | 
| primaryPersonName | string | 256 | profile | 
| primaryPersonFirstName | string | 64 | profile | 
| primaryPersonLastName | string | 64 | profile | 
| primaryPersonEmail | string | 256 | profile | 
| primaryPersonPhone | string | 256 | profile | 
| clientAnniversaryDay | short |  | clientProfile | 
| clientAnniversaryMonth | short |  | clientProfile | 
| clientAnniversaryYear | short |  | clientProfile | 
| clientAnniversaryNote | string | 256 | clientProfile | 
| clientAdvisorProfileRecNo | long |  | clientProfile | 
| clientAdvisorName | string | 256 | clientProfile | 
| clientBranchRecNo | long |  | clientProfile | 
| clientBranchName | string | 64 | clientProfile | 
| remarks | string | 256 | profile | 
| activeStatus | bool |  | profile | 
| primaryEmail | string | 256 | profile | 
| primaryEmailPermitMarketing | bool |  | profile | 
| primaryPhone | string | 256 | profile | 
| primaryPhonePermitMarketing | bool |  | profile | 
| preferredSupplier | bool |  | supplierProfile | 
| street1 | string | 128 | address | 
| street2 | string | 128 | address | 
| city | string | 64 | address | 
| stateProvince | string | 8 | address | 
| zipPostalCode | string | 16 | address | 
| country | string | 4 | address | 
| mailingStreet1 | string | 128 | address | 
| mailingStreet2 | string | 128 | address | 
| mailingCity | string | 64 | address | 
| mailingStateProvince | string | 8 | address | 
| mailingZipPostalCode | string | 16 | address | 
| mailingCountry | string | 4 | address | 
| addressPermitMarketing | bool |  | address | 
| clientReferredBy | string | 64 | clientProfile | 
| clientCreateDateTime | DateTime |  | clientProfile | 
| clientLastModifiedDateTime | DateTime |  | clientProfile | 
| supplierVendorId | string | 10 | supplierProfile | 
| clientInformalSalutation | string | 128 | clientProfile | 
| clientFormalSalutation | string | 128 | clientProfile | 

| Parameter | Type | Linked Parameter | Description |
| --------- | ---- | ---------------- | ----------- |
| recNo [inherited] | long |  | 
| recNoList [inherited] | long[] |  | 
| startingRow [inherited] | int |  | 
| rowCount [inherited] | int |  | 
| topRows [inherited] | int |  | 
| distinct [inherited] | bool |  | 
| includeCols [inherited] | string[] |  | 
| includeColsExtended [inherited] | [includeColsExtended[]](/includeColsExtended) |  | 
| baseUrl [inherited] | string |  | 
| tagRecNo [inherited] | long[] |  | 
| tagValueCond [inherited] | short |  | 
| tagValue [inherited] | string |  | 
| displayTagRecNo [inherited] | long |  | 
| tags [inherited] | [TagsSearch[]](/TagsSearch) |  | 
| profileType | short |  | 
| profileName | string |  | 
| profileNameCond | short |  | 
| commType | short |  | 
| commValue | string |  | 
| commValueCond | short |  | 
| clientAnniversaryMonth | short[] |  | 
| clientAnniversaryMonthFrom | short |  | 
| clientAnniversaryMonthTo | short |  | 
| clientAnniversaryDayFrom | short |  | 
| clientAnniversaryDayTo | short |  | 
| clientAdvisorProfileRecNo | long |  | 
| clientType | short |  | 
| supplierType | short |  | 
| activestatus | bool |  | 
| clientBranchRecNo | long |  | 
| personRecNo | long |  | 
| personName | string |  | 
| personFirstName | string |  | 
| personFirstNameCond | short |  | 
| personLastName | string |  | 
| personLastNameCond | short |  | 
| preferredSupplier | bool |  | 
| street1 | string |  | 
| city | string |  | 
| stateProvince | string |  | 
| zipPostalCode | string |  | 
| country | string |  | 
| marketing | [marketing[]](/marketing) |  | 
| id | string |  | 
| emailPermitMarketing | bool |  | 
| phonePermitMarketing | bool |  | 
| addressPermitMarketing | bool |  | 
| clientCreateDateTimeFrom | DateTimeOffset |  | 
| clientCreateDateTimeTo | DateTimeOffset |  | 
| clientModifiedDateTimeFrom | DateTimeOffset |  | 
| clientModifiedDateTimeTo | DateTimeOffset |  | 
| supplierVendorId | string |  | 
| clientTripSearchParams | [tripSearch](/tripSearch) |  | 
| supplierTripSearchParams | [tripSearch](/tripSearch) |  | 
| clientActivitySearchParams | [activitySearch](/activitySearch) |  | 

| Status code | Description |
| ----------- | ----------- |
| 200 | Ok |
| 401 | Unauthorized |
| 403 | Forbidden |

#### Example request
```sh
POST https://api-dev.trestechnologies.com/profileSearch
Content-Type: application/json
Authorization: Bearer <session-token>
```

#### Example response
```sh
Content-Type: application/json
Status: 200 Ok
```