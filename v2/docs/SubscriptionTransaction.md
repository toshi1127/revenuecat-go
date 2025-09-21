# SubscriptionTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The ID of the subscription transaction in the store | 
**PurchasedAt** | **int64** | The date of the transaction in ms since epoch | 

## Methods

### NewSubscriptionTransaction

`func NewSubscriptionTransaction(object string, id string, purchasedAt int64, ) *SubscriptionTransaction`

NewSubscriptionTransaction instantiates a new SubscriptionTransaction object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSubscriptionTransactionWithDefaults

`func NewSubscriptionTransactionWithDefaults() *SubscriptionTransaction`

NewSubscriptionTransactionWithDefaults instantiates a new SubscriptionTransaction object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *SubscriptionTransaction) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *SubscriptionTransaction) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *SubscriptionTransaction) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *SubscriptionTransaction) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SubscriptionTransaction) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SubscriptionTransaction) SetId(v string)`

SetId sets Id field to given value.


### GetPurchasedAt

`func (o *SubscriptionTransaction) GetPurchasedAt() int64`

GetPurchasedAt returns the PurchasedAt field if non-nil, zero value otherwise.

### GetPurchasedAtOk

`func (o *SubscriptionTransaction) GetPurchasedAtOk() (*int64, bool)`

GetPurchasedAtOk returns a tuple with the PurchasedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPurchasedAt

`func (o *SubscriptionTransaction) SetPurchasedAt(v int64)`

SetPurchasedAt sets PurchasedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


