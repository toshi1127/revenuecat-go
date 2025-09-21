# VirtualCurrencyBalance

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**CurrencyCode** | **string** | The code of the virtual currency. | 
**Balance** | **int32** | The balance of the virtual currency. | 

## Methods

### NewVirtualCurrencyBalance

`func NewVirtualCurrencyBalance(object string, currencyCode string, balance int32, ) *VirtualCurrencyBalance`

NewVirtualCurrencyBalance instantiates a new VirtualCurrencyBalance object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVirtualCurrencyBalanceWithDefaults

`func NewVirtualCurrencyBalanceWithDefaults() *VirtualCurrencyBalance`

NewVirtualCurrencyBalanceWithDefaults instantiates a new VirtualCurrencyBalance object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *VirtualCurrencyBalance) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *VirtualCurrencyBalance) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *VirtualCurrencyBalance) SetObject(v string)`

SetObject sets Object field to given value.


### GetCurrencyCode

`func (o *VirtualCurrencyBalance) GetCurrencyCode() string`

GetCurrencyCode returns the CurrencyCode field if non-nil, zero value otherwise.

### GetCurrencyCodeOk

`func (o *VirtualCurrencyBalance) GetCurrencyCodeOk() (*string, bool)`

GetCurrencyCodeOk returns a tuple with the CurrencyCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyCode

`func (o *VirtualCurrencyBalance) SetCurrencyCode(v string)`

SetCurrencyCode sets CurrencyCode field to given value.


### GetBalance

`func (o *VirtualCurrencyBalance) GetBalance() int32`

GetBalance returns the Balance field if non-nil, zero value otherwise.

### GetBalanceOk

`func (o *VirtualCurrencyBalance) GetBalanceOk() (*int32, bool)`

GetBalanceOk returns a tuple with the Balance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalance

`func (o *VirtualCurrencyBalance) SetBalance(v int32)`

SetBalance sets Balance field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


