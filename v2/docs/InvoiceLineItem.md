# InvoiceLineItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**ProductIdentifier** | **string** | The product identifier | 
**ProductDisplayName** | **NullableString** | The display name of the product | 
**ProductDuration** | **NullableString** | The duration of the subscription in ISO-8601 standard | 
**Quantity** | **int32** | Total purchased items | 
**UnitAmount** | [**MonetaryAmount**](MonetaryAmount.md) |  | 

## Methods

### NewInvoiceLineItem

`func NewInvoiceLineItem(object string, productIdentifier string, productDisplayName NullableString, productDuration NullableString, quantity int32, unitAmount MonetaryAmount, ) *InvoiceLineItem`

NewInvoiceLineItem instantiates a new InvoiceLineItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceLineItemWithDefaults

`func NewInvoiceLineItemWithDefaults() *InvoiceLineItem`

NewInvoiceLineItemWithDefaults instantiates a new InvoiceLineItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *InvoiceLineItem) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *InvoiceLineItem) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *InvoiceLineItem) SetObject(v string)`

SetObject sets Object field to given value.


### GetProductIdentifier

`func (o *InvoiceLineItem) GetProductIdentifier() string`

GetProductIdentifier returns the ProductIdentifier field if non-nil, zero value otherwise.

### GetProductIdentifierOk

`func (o *InvoiceLineItem) GetProductIdentifierOk() (*string, bool)`

GetProductIdentifierOk returns a tuple with the ProductIdentifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductIdentifier

`func (o *InvoiceLineItem) SetProductIdentifier(v string)`

SetProductIdentifier sets ProductIdentifier field to given value.


### GetProductDisplayName

`func (o *InvoiceLineItem) GetProductDisplayName() string`

GetProductDisplayName returns the ProductDisplayName field if non-nil, zero value otherwise.

### GetProductDisplayNameOk

`func (o *InvoiceLineItem) GetProductDisplayNameOk() (*string, bool)`

GetProductDisplayNameOk returns a tuple with the ProductDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductDisplayName

`func (o *InvoiceLineItem) SetProductDisplayName(v string)`

SetProductDisplayName sets ProductDisplayName field to given value.


### SetProductDisplayNameNil

`func (o *InvoiceLineItem) SetProductDisplayNameNil(b bool)`

 SetProductDisplayNameNil sets the value for ProductDisplayName to be an explicit nil

### UnsetProductDisplayName
`func (o *InvoiceLineItem) UnsetProductDisplayName()`

UnsetProductDisplayName ensures that no value is present for ProductDisplayName, not even an explicit nil
### GetProductDuration

`func (o *InvoiceLineItem) GetProductDuration() string`

GetProductDuration returns the ProductDuration field if non-nil, zero value otherwise.

### GetProductDurationOk

`func (o *InvoiceLineItem) GetProductDurationOk() (*string, bool)`

GetProductDurationOk returns a tuple with the ProductDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductDuration

`func (o *InvoiceLineItem) SetProductDuration(v string)`

SetProductDuration sets ProductDuration field to given value.


### SetProductDurationNil

`func (o *InvoiceLineItem) SetProductDurationNil(b bool)`

 SetProductDurationNil sets the value for ProductDuration to be an explicit nil

### UnsetProductDuration
`func (o *InvoiceLineItem) UnsetProductDuration()`

UnsetProductDuration ensures that no value is present for ProductDuration, not even an explicit nil
### GetQuantity

`func (o *InvoiceLineItem) GetQuantity() int32`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *InvoiceLineItem) GetQuantityOk() (*int32, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *InvoiceLineItem) SetQuantity(v int32)`

SetQuantity sets Quantity field to given value.


### GetUnitAmount

`func (o *InvoiceLineItem) GetUnitAmount() MonetaryAmount`

GetUnitAmount returns the UnitAmount field if non-nil, zero value otherwise.

### GetUnitAmountOk

`func (o *InvoiceLineItem) GetUnitAmountOk() (*MonetaryAmount, bool)`

GetUnitAmountOk returns a tuple with the UnitAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnitAmount

`func (o *InvoiceLineItem) SetUnitAmount(v MonetaryAmount)`

SetUnitAmount sets UnitAmount field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


