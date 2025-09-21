# StoreProduct

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The unique identifier of the product in the store (e.g., App Store Connect product ID) | 
**Name** | Pointer to **NullableString** | The name of the store product | [optional] 
**ProductIdentifier** | **string** | The product identifier used in the store | 

## Methods

### NewStoreProduct

`func NewStoreProduct(object string, id string, productIdentifier string, ) *StoreProduct`

NewStoreProduct instantiates a new StoreProduct object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStoreProductWithDefaults

`func NewStoreProductWithDefaults() *StoreProduct`

NewStoreProductWithDefaults instantiates a new StoreProduct object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *StoreProduct) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *StoreProduct) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *StoreProduct) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *StoreProduct) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *StoreProduct) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *StoreProduct) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *StoreProduct) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *StoreProduct) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *StoreProduct) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *StoreProduct) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *StoreProduct) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *StoreProduct) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetProductIdentifier

`func (o *StoreProduct) GetProductIdentifier() string`

GetProductIdentifier returns the ProductIdentifier field if non-nil, zero value otherwise.

### GetProductIdentifierOk

`func (o *StoreProduct) GetProductIdentifierOk() (*string, bool)`

GetProductIdentifierOk returns a tuple with the ProductIdentifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductIdentifier

`func (o *StoreProduct) SetProductIdentifier(v string)`

SetProductIdentifier sets ProductIdentifier field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


