# CustomerEntitlement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**EntitlementId** | **string** | ID of the entitlement granted to the customer | 
**ExpiresAt** | **NullableInt64** | The date after which the access to the entitlement expires in ms since epoch | 

## Methods

### NewCustomerEntitlement

`func NewCustomerEntitlement(object string, entitlementId string, expiresAt NullableInt64, ) *CustomerEntitlement`

NewCustomerEntitlement instantiates a new CustomerEntitlement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCustomerEntitlementWithDefaults

`func NewCustomerEntitlementWithDefaults() *CustomerEntitlement`

NewCustomerEntitlementWithDefaults instantiates a new CustomerEntitlement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *CustomerEntitlement) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *CustomerEntitlement) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *CustomerEntitlement) SetObject(v string)`

SetObject sets Object field to given value.


### GetEntitlementId

`func (o *CustomerEntitlement) GetEntitlementId() string`

GetEntitlementId returns the EntitlementId field if non-nil, zero value otherwise.

### GetEntitlementIdOk

`func (o *CustomerEntitlement) GetEntitlementIdOk() (*string, bool)`

GetEntitlementIdOk returns a tuple with the EntitlementId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntitlementId

`func (o *CustomerEntitlement) SetEntitlementId(v string)`

SetEntitlementId sets EntitlementId field to given value.


### GetExpiresAt

`func (o *CustomerEntitlement) GetExpiresAt() int64`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *CustomerEntitlement) GetExpiresAtOk() (*int64, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *CustomerEntitlement) SetExpiresAt(v int64)`

SetExpiresAt sets ExpiresAt field to given value.


### SetExpiresAtNil

`func (o *CustomerEntitlement) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *CustomerEntitlement) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


