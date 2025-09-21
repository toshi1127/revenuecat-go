# ProductsFromEntitlement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. Always has the value &#x60;list&#x60;. | 
**Items** | [**[]Product**](Product.md) | Details about each object. | 
**NextPage** | **NullableString** | URL to access the next page of the entitlement&#39;s products. If not present / null, there is no next page | 
**Url** | **string** | The URL where this list can be accessed. | 

## Methods

### NewProductsFromEntitlement

`func NewProductsFromEntitlement(object string, items []Product, nextPage NullableString, url string, ) *ProductsFromEntitlement`

NewProductsFromEntitlement instantiates a new ProductsFromEntitlement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductsFromEntitlementWithDefaults

`func NewProductsFromEntitlementWithDefaults() *ProductsFromEntitlement`

NewProductsFromEntitlementWithDefaults instantiates a new ProductsFromEntitlement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *ProductsFromEntitlement) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *ProductsFromEntitlement) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *ProductsFromEntitlement) SetObject(v string)`

SetObject sets Object field to given value.


### GetItems

`func (o *ProductsFromEntitlement) GetItems() []Product`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *ProductsFromEntitlement) GetItemsOk() (*[]Product, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *ProductsFromEntitlement) SetItems(v []Product)`

SetItems sets Items field to given value.


### GetNextPage

`func (o *ProductsFromEntitlement) GetNextPage() string`

GetNextPage returns the NextPage field if non-nil, zero value otherwise.

### GetNextPageOk

`func (o *ProductsFromEntitlement) GetNextPageOk() (*string, bool)`

GetNextPageOk returns a tuple with the NextPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPage

`func (o *ProductsFromEntitlement) SetNextPage(v string)`

SetNextPage sets NextPage field to given value.


### SetNextPageNil

`func (o *ProductsFromEntitlement) SetNextPageNil(b bool)`

 SetNextPageNil sets the value for NextPage to be an explicit nil

### UnsetNextPage
`func (o *ProductsFromEntitlement) UnsetNextPage()`

UnsetNextPage ensures that no value is present for NextPage, not even an explicit nil
### GetUrl

`func (o *ProductsFromEntitlement) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *ProductsFromEntitlement) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *ProductsFromEntitlement) SetUrl(v string)`

SetUrl sets Url field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


