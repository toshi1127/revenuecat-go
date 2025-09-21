# Invoice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The id of the invoice | 
**TotalAmount** | [**MonetaryAmount**](MonetaryAmount.md) |  | 
**LineItems** | [**[]InvoiceLineItem**](InvoiceLineItem.md) | List of line items that are part of the invoice. Each line item represents a product that was purchased. | 
**IssuedAt** | **int64** | The date when the invoiced was issued in ms since epoch | 
**PaidAt** | **NullableInt64** | The date when the invoiced was paid in ms since epoch | 
**InvoiceUrl** | **NullableString** | URL to download the invoice pdf | 

## Methods

### NewInvoice

`func NewInvoice(object string, id string, totalAmount MonetaryAmount, lineItems []InvoiceLineItem, issuedAt int64, paidAt NullableInt64, invoiceUrl NullableString, ) *Invoice`

NewInvoice instantiates a new Invoice object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInvoiceWithDefaults

`func NewInvoiceWithDefaults() *Invoice`

NewInvoiceWithDefaults instantiates a new Invoice object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Invoice) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Invoice) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Invoice) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *Invoice) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Invoice) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Invoice) SetId(v string)`

SetId sets Id field to given value.


### GetTotalAmount

`func (o *Invoice) GetTotalAmount() MonetaryAmount`

GetTotalAmount returns the TotalAmount field if non-nil, zero value otherwise.

### GetTotalAmountOk

`func (o *Invoice) GetTotalAmountOk() (*MonetaryAmount, bool)`

GetTotalAmountOk returns a tuple with the TotalAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalAmount

`func (o *Invoice) SetTotalAmount(v MonetaryAmount)`

SetTotalAmount sets TotalAmount field to given value.


### GetLineItems

`func (o *Invoice) GetLineItems() []InvoiceLineItem`

GetLineItems returns the LineItems field if non-nil, zero value otherwise.

### GetLineItemsOk

`func (o *Invoice) GetLineItemsOk() (*[]InvoiceLineItem, bool)`

GetLineItemsOk returns a tuple with the LineItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLineItems

`func (o *Invoice) SetLineItems(v []InvoiceLineItem)`

SetLineItems sets LineItems field to given value.


### GetIssuedAt

`func (o *Invoice) GetIssuedAt() int64`

GetIssuedAt returns the IssuedAt field if non-nil, zero value otherwise.

### GetIssuedAtOk

`func (o *Invoice) GetIssuedAtOk() (*int64, bool)`

GetIssuedAtOk returns a tuple with the IssuedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuedAt

`func (o *Invoice) SetIssuedAt(v int64)`

SetIssuedAt sets IssuedAt field to given value.


### GetPaidAt

`func (o *Invoice) GetPaidAt() int64`

GetPaidAt returns the PaidAt field if non-nil, zero value otherwise.

### GetPaidAtOk

`func (o *Invoice) GetPaidAtOk() (*int64, bool)`

GetPaidAtOk returns a tuple with the PaidAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaidAt

`func (o *Invoice) SetPaidAt(v int64)`

SetPaidAt sets PaidAt field to given value.


### SetPaidAtNil

`func (o *Invoice) SetPaidAtNil(b bool)`

 SetPaidAtNil sets the value for PaidAt to be an explicit nil

### UnsetPaidAt
`func (o *Invoice) UnsetPaidAt()`

UnsetPaidAt ensures that no value is present for PaidAt, not even an explicit nil
### GetInvoiceUrl

`func (o *Invoice) GetInvoiceUrl() string`

GetInvoiceUrl returns the InvoiceUrl field if non-nil, zero value otherwise.

### GetInvoiceUrlOk

`func (o *Invoice) GetInvoiceUrlOk() (*string, bool)`

GetInvoiceUrlOk returns a tuple with the InvoiceUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInvoiceUrl

`func (o *Invoice) SetInvoiceUrl(v string)`

SetInvoiceUrl sets InvoiceUrl field to given value.


### SetInvoiceUrlNil

`func (o *Invoice) SetInvoiceUrlNil(b bool)`

 SetInvoiceUrlNil sets the value for InvoiceUrl to be an explicit nil

### UnsetInvoiceUrl
`func (o *Invoice) UnsetInvoiceUrl()`

UnsetInvoiceUrl ensures that no value is present for InvoiceUrl, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


