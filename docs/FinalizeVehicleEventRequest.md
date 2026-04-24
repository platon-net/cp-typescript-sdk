# FinalizeVehicleEventRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**eventType** | **string** |  | [default to undefined]
**datetimeLocal** | **string** |  | [default to undefined]
**timezone** | **string** |  | [default to undefined]
**location** | [**FinalizeVehicleEventRequestLocation**](FinalizeVehicleEventRequestLocation.md) |  | [default to undefined]
**purpose** | **string** |  | [optional] [default to undefined]
**notes** | **string** |  | [optional] [default to undefined]
**odometer** | **number** |  | [optional] [default to undefined]
**money** | [**FinalizeVehicleEventRequestMoney**](FinalizeVehicleEventRequestMoney.md) |  | [optional] [default to undefined]
**fueling** | [**FinalizeVehicleEventRequestFueling**](FinalizeVehicleEventRequestFueling.md) |  | [optional] [default to undefined]

## Example

```typescript
import { FinalizeVehicleEventRequest } from 'cp-typescript-sdk';

const instance: FinalizeVehicleEventRequest = {
    eventType,
    datetimeLocal,
    timezone,
    location,
    purpose,
    notes,
    odometer,
    money,
    fueling,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
