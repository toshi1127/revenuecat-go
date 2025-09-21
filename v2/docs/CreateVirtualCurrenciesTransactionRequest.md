# CreateVirtualCurrenciesTransactionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Adjustments** | **map[string]int32** | The adjustments to the virtual currencies | 
**Reference** | Pointer to **NullableString** | The reference of the transaction | [optional] 

## Methods

### NewCreateVirtualCurrenciesTransactionRequest

`func NewCreateVirtualCurrenciesTransactionRequest(adjustments map[string]int32, ) *CreateVirtualCurrenciesTransactionRequest`

NewCreateVirtualCurrenciesTransactionRequest instantiates a new CreateVirtualCurrenciesTransactionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateVirtualCurrenciesTransactionRequestWithDefaults

`func NewCreateVirtualCurrenciesTransactionRequestWithDefaults() *CreateVirtualCurrenciesTransactionRequest`

NewCreateVirtualCurrenciesTransactionRequestWithDefaults instantiates a new CreateVirtualCurrenciesTransactionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAdjustments

`func (o *CreateVirtualCurrenciesTransactionRequest) GetAdjustments() map[string]int32`

GetAdjustments returns the Adjustments field if non-nil, zero value otherwise.

### GetAdjustmentsOk

`func (o *CreateVirtualCurrenciesTransactionRequest) GetAdjustmentsOk() (*map[string]int32, bool)`

GetAdjustmentsOk returns a tuple with the Adjustments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAdjustments

`func (o *CreateVirtualCurrenciesTransactionRequest) SetAdjustments(v map[string]int32)`

SetAdjustments sets Adjustments field to given value.


### GetReference

`func (o *CreateVirtualCurrenciesTransactionRequest) GetReference() string`

GetReference returns the Reference field if non-nil, zero value otherwise.

### GetReferenceOk

`func (o *CreateVirtualCurrenciesTransactionRequest) GetReferenceOk() (*string, bool)`

GetReferenceOk returns a tuple with the Reference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReference

`func (o *CreateVirtualCurrenciesTransactionRequest) SetReference(v string)`

SetReference sets Reference field to given value.

### HasReference

`func (o *CreateVirtualCurrenciesTransactionRequest) HasReference() bool`

HasReference returns a boolean if a field has been set.

### SetReferenceNil

`func (o *CreateVirtualCurrenciesTransactionRequest) SetReferenceNil(b bool)`

 SetReferenceNil sets the value for Reference to be an explicit nil

### UnsetReference
`func (o *CreateVirtualCurrenciesTransactionRequest) UnsetReference()`

UnsetReference ensures that no value is present for Reference, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


