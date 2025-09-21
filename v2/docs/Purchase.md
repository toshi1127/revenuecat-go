# Purchase

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The id of the purchase | 
**CustomerId** | **string** | The id of the customer | 
**OriginalCustomerId** | **string** | The ID of the original customer | 
**ProductId** | **string** | The ID of the product that was purchased | 
**PurchasedAt** | **int64** | The date when the purchase was made in ms since epoch | 
**RevenueInUsd** | [**MonetaryAmount**](MonetaryAmount.md) |  | 
**Quantity** | **int32** | The quantity of the product purchased in one transaction | 
**Status** | **string** | The status of a purchase | 
**PresentedOfferingId** | **NullableString** | The ID of the offering the customer saw when they did the purchase | 
**Entitlements** | [**EntitlementList**](EntitlementList.md) |  | 
**Environment** | [**Environment**](Environment.md) |  | 
**Store** | **string** | Store the purchase belongs to | 
**StorePurchaseIdentifier** | **string** | The store purchase identifier | 
**Ownership** | [**Ownership**](Ownership.md) |  | 
**Country** | Pointer to [**NullableCountry**](Country.md) |  | [optional] 

## Methods

### NewPurchase

`func NewPurchase(object string, id string, customerId string, originalCustomerId string, productId string, purchasedAt int64, revenueInUsd MonetaryAmount, quantity int32, status string, presentedOfferingId NullableString, entitlements EntitlementList, environment Environment, store string, storePurchaseIdentifier string, ownership Ownership, ) *Purchase`

NewPurchase instantiates a new Purchase object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPurchaseWithDefaults

`func NewPurchaseWithDefaults() *Purchase`

NewPurchaseWithDefaults instantiates a new Purchase object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Purchase) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Purchase) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Purchase) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *Purchase) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Purchase) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Purchase) SetId(v string)`

SetId sets Id field to given value.


### GetCustomerId

`func (o *Purchase) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *Purchase) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *Purchase) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetOriginalCustomerId

`func (o *Purchase) GetOriginalCustomerId() string`

GetOriginalCustomerId returns the OriginalCustomerId field if non-nil, zero value otherwise.

### GetOriginalCustomerIdOk

`func (o *Purchase) GetOriginalCustomerIdOk() (*string, bool)`

GetOriginalCustomerIdOk returns a tuple with the OriginalCustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalCustomerId

`func (o *Purchase) SetOriginalCustomerId(v string)`

SetOriginalCustomerId sets OriginalCustomerId field to given value.


### GetProductId

`func (o *Purchase) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *Purchase) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *Purchase) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetPurchasedAt

`func (o *Purchase) GetPurchasedAt() int64`

GetPurchasedAt returns the PurchasedAt field if non-nil, zero value otherwise.

### GetPurchasedAtOk

`func (o *Purchase) GetPurchasedAtOk() (*int64, bool)`

GetPurchasedAtOk returns a tuple with the PurchasedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPurchasedAt

`func (o *Purchase) SetPurchasedAt(v int64)`

SetPurchasedAt sets PurchasedAt field to given value.


### GetRevenueInUsd

`func (o *Purchase) GetRevenueInUsd() MonetaryAmount`

GetRevenueInUsd returns the RevenueInUsd field if non-nil, zero value otherwise.

### GetRevenueInUsdOk

`func (o *Purchase) GetRevenueInUsdOk() (*MonetaryAmount, bool)`

GetRevenueInUsdOk returns a tuple with the RevenueInUsd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevenueInUsd

`func (o *Purchase) SetRevenueInUsd(v MonetaryAmount)`

SetRevenueInUsd sets RevenueInUsd field to given value.


### GetQuantity

`func (o *Purchase) GetQuantity() int32`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *Purchase) GetQuantityOk() (*int32, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *Purchase) SetQuantity(v int32)`

SetQuantity sets Quantity field to given value.


### GetStatus

`func (o *Purchase) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Purchase) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Purchase) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetPresentedOfferingId

`func (o *Purchase) GetPresentedOfferingId() string`

GetPresentedOfferingId returns the PresentedOfferingId field if non-nil, zero value otherwise.

### GetPresentedOfferingIdOk

`func (o *Purchase) GetPresentedOfferingIdOk() (*string, bool)`

GetPresentedOfferingIdOk returns a tuple with the PresentedOfferingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresentedOfferingId

`func (o *Purchase) SetPresentedOfferingId(v string)`

SetPresentedOfferingId sets PresentedOfferingId field to given value.


### SetPresentedOfferingIdNil

`func (o *Purchase) SetPresentedOfferingIdNil(b bool)`

 SetPresentedOfferingIdNil sets the value for PresentedOfferingId to be an explicit nil

### UnsetPresentedOfferingId
`func (o *Purchase) UnsetPresentedOfferingId()`

UnsetPresentedOfferingId ensures that no value is present for PresentedOfferingId, not even an explicit nil
### GetEntitlements

`func (o *Purchase) GetEntitlements() EntitlementList`

GetEntitlements returns the Entitlements field if non-nil, zero value otherwise.

### GetEntitlementsOk

`func (o *Purchase) GetEntitlementsOk() (*EntitlementList, bool)`

GetEntitlementsOk returns a tuple with the Entitlements field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntitlements

`func (o *Purchase) SetEntitlements(v EntitlementList)`

SetEntitlements sets Entitlements field to given value.


### GetEnvironment

`func (o *Purchase) GetEnvironment() Environment`

GetEnvironment returns the Environment field if non-nil, zero value otherwise.

### GetEnvironmentOk

`func (o *Purchase) GetEnvironmentOk() (*Environment, bool)`

GetEnvironmentOk returns a tuple with the Environment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironment

`func (o *Purchase) SetEnvironment(v Environment)`

SetEnvironment sets Environment field to given value.


### GetStore

`func (o *Purchase) GetStore() string`

GetStore returns the Store field if non-nil, zero value otherwise.

### GetStoreOk

`func (o *Purchase) GetStoreOk() (*string, bool)`

GetStoreOk returns a tuple with the Store field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStore

`func (o *Purchase) SetStore(v string)`

SetStore sets Store field to given value.


### GetStorePurchaseIdentifier

`func (o *Purchase) GetStorePurchaseIdentifier() string`

GetStorePurchaseIdentifier returns the StorePurchaseIdentifier field if non-nil, zero value otherwise.

### GetStorePurchaseIdentifierOk

`func (o *Purchase) GetStorePurchaseIdentifierOk() (*string, bool)`

GetStorePurchaseIdentifierOk returns a tuple with the StorePurchaseIdentifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStorePurchaseIdentifier

`func (o *Purchase) SetStorePurchaseIdentifier(v string)`

SetStorePurchaseIdentifier sets StorePurchaseIdentifier field to given value.


### GetOwnership

`func (o *Purchase) GetOwnership() Ownership`

GetOwnership returns the Ownership field if non-nil, zero value otherwise.

### GetOwnershipOk

`func (o *Purchase) GetOwnershipOk() (*Ownership, bool)`

GetOwnershipOk returns a tuple with the Ownership field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnership

`func (o *Purchase) SetOwnership(v Ownership)`

SetOwnership sets Ownership field to given value.


### GetCountry

`func (o *Purchase) GetCountry() Country`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *Purchase) GetCountryOk() (*Country, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *Purchase) SetCountry(v Country)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *Purchase) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### SetCountryNil

`func (o *Purchase) SetCountryNil(b bool)`

 SetCountryNil sets the value for Country to be an explicit nil

### UnsetCountry
`func (o *Purchase) UnsetCountry()`

UnsetCountry ensures that no value is present for Country, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


