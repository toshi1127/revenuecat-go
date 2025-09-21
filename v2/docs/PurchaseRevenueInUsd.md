# PurchaseRevenueInUsd

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Currency** | [**Currency**](Currency.md) |  | 
**Gross** | **float32** | Total revenue generated (excluding taxes and commission) | 
**Commission** | Pointer to **float32** | Store commission or payment processor fees deducted from gross revenue (if any) | [optional] 
**Tax** | **float32** | Estimated taxes deducted from gross revenue | 
**Proceeds** | **float32** | Net revenue after store commission / fees and taxes | 

## Methods

### NewPurchaseRevenueInUsd

`func NewPurchaseRevenueInUsd(currency Currency, gross float32, tax float32, proceeds float32, ) *PurchaseRevenueInUsd`

NewPurchaseRevenueInUsd instantiates a new PurchaseRevenueInUsd object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPurchaseRevenueInUsdWithDefaults

`func NewPurchaseRevenueInUsdWithDefaults() *PurchaseRevenueInUsd`

NewPurchaseRevenueInUsdWithDefaults instantiates a new PurchaseRevenueInUsd object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrency

`func (o *PurchaseRevenueInUsd) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *PurchaseRevenueInUsd) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *PurchaseRevenueInUsd) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.


### GetGross

`func (o *PurchaseRevenueInUsd) GetGross() float32`

GetGross returns the Gross field if non-nil, zero value otherwise.

### GetGrossOk

`func (o *PurchaseRevenueInUsd) GetGrossOk() (*float32, bool)`

GetGrossOk returns a tuple with the Gross field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGross

`func (o *PurchaseRevenueInUsd) SetGross(v float32)`

SetGross sets Gross field to given value.


### GetCommission

`func (o *PurchaseRevenueInUsd) GetCommission() float32`

GetCommission returns the Commission field if non-nil, zero value otherwise.

### GetCommissionOk

`func (o *PurchaseRevenueInUsd) GetCommissionOk() (*float32, bool)`

GetCommissionOk returns a tuple with the Commission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCommission

`func (o *PurchaseRevenueInUsd) SetCommission(v float32)`

SetCommission sets Commission field to given value.

### HasCommission

`func (o *PurchaseRevenueInUsd) HasCommission() bool`

HasCommission returns a boolean if a field has been set.

### GetTax

`func (o *PurchaseRevenueInUsd) GetTax() float32`

GetTax returns the Tax field if non-nil, zero value otherwise.

### GetTaxOk

`func (o *PurchaseRevenueInUsd) GetTaxOk() (*float32, bool)`

GetTaxOk returns a tuple with the Tax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTax

`func (o *PurchaseRevenueInUsd) SetTax(v float32)`

SetTax sets Tax field to given value.


### GetProceeds

`func (o *PurchaseRevenueInUsd) GetProceeds() float32`

GetProceeds returns the Proceeds field if non-nil, zero value otherwise.

### GetProceedsOk

`func (o *PurchaseRevenueInUsd) GetProceedsOk() (*float32, bool)`

GetProceedsOk returns a tuple with the Proceeds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProceeds

`func (o *PurchaseRevenueInUsd) SetProceeds(v float32)`

SetProceeds sets Proceeds field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


