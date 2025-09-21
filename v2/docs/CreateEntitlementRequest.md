# CreateEntitlementRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LookupKey** | **string** | The identifier of the entitlement | 
**DisplayName** | **string** | The display name of the entitlement | 

## Methods

### NewCreateEntitlementRequest

`func NewCreateEntitlementRequest(lookupKey string, displayName string, ) *CreateEntitlementRequest`

NewCreateEntitlementRequest instantiates a new CreateEntitlementRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateEntitlementRequestWithDefaults

`func NewCreateEntitlementRequestWithDefaults() *CreateEntitlementRequest`

NewCreateEntitlementRequestWithDefaults instantiates a new CreateEntitlementRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLookupKey

`func (o *CreateEntitlementRequest) GetLookupKey() string`

GetLookupKey returns the LookupKey field if non-nil, zero value otherwise.

### GetLookupKeyOk

`func (o *CreateEntitlementRequest) GetLookupKeyOk() (*string, bool)`

GetLookupKeyOk returns a tuple with the LookupKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLookupKey

`func (o *CreateEntitlementRequest) SetLookupKey(v string)`

SetLookupKey sets LookupKey field to given value.


### GetDisplayName

`func (o *CreateEntitlementRequest) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *CreateEntitlementRequest) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *CreateEntitlementRequest) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


