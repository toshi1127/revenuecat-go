# MonetaryAmount

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Currency** | [**Currency**](Currency.md) |  | 
**Gross** | **float32** | Total revenue generated (excluding taxes and commission) | 
**Commission** | Pointer to **float32** | Store commission or payment processor fees deducted from gross revenue (if any) | [optional] 
**Tax** | **float32** | Estimated taxes deducted from gross revenue | 
**Proceeds** | **float32** | Net revenue after store commission / fees and taxes | 

## Methods

### NewMonetaryAmount

`func NewMonetaryAmount(currency Currency, gross float32, tax float32, proceeds float32, ) *MonetaryAmount`

NewMonetaryAmount instantiates a new MonetaryAmount object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMonetaryAmountWithDefaults

`func NewMonetaryAmountWithDefaults() *MonetaryAmount`

NewMonetaryAmountWithDefaults instantiates a new MonetaryAmount object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrency

`func (o *MonetaryAmount) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *MonetaryAmount) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *MonetaryAmount) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.


### GetGross

`func (o *MonetaryAmount) GetGross() float32`

GetGross returns the Gross field if non-nil, zero value otherwise.

### GetGrossOk

`func (o *MonetaryAmount) GetGrossOk() (*float32, bool)`

GetGrossOk returns a tuple with the Gross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGross

`func (o *MonetaryAmount) SetGross(v float32)`

SetGross sets Gross field to given value.


### GetCommission

`func (o *MonetaryAmount) GetCommission() float32`

GetCommission returns the Commission field if non-nil, zero value otherwise.

### GetCommissionOk

`func (o *MonetaryAmount) GetCommissionOk() (*float32, bool)`

GetCommissionOk returns a tuple with the Commission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommission

`func (o *MonetaryAmount) SetCommission(v float32)`

SetCommission sets Commission field to given value.

### HasCommission

`func (o *MonetaryAmount) HasCommission() bool`

HasCommission returns a boolean if a field has been set.

### GetTax

`func (o *MonetaryAmount) GetTax() float32`

GetTax returns the Tax field if non-nil, zero value otherwise.

### GetTaxOk

`func (o *MonetaryAmount) GetTaxOk() (*float32, bool)`

GetTaxOk returns a tuple with the Tax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTax

`func (o *MonetaryAmount) SetTax(v float32)`

SetTax sets Tax field to given value.


### GetProceeds

`func (o *MonetaryAmount) GetProceeds() float32`

GetProceeds returns the Proceeds field if non-nil, zero value otherwise.

### GetProceedsOk

`func (o *MonetaryAmount) GetProceedsOk() (*float32, bool)`

GetProceedsOk returns a tuple with the Proceeds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProceeds

`func (o *MonetaryAmount) SetProceeds(v float32)`

SetProceeds sets Proceeds field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


