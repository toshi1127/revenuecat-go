# Package

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The id of the package | 
**LookupKey** | **string** | The lookup_key of the package | 
**DisplayName** | **string** | The display name of the package | 
**Position** | **NullableInt32** | The position of the package within the offering | 
**CreatedAt** | **int64** | The date the package was created at in ms since epoch | 
**Products** | Pointer to [**NullableProductList**](ProductList.md) |  | [optional] 

## Methods

### NewPackage

`func NewPackage(object string, id string, lookupKey string, displayName string, position NullableInt32, createdAt int64, ) *Package`

NewPackage instantiates a new Package object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPackageWithDefaults

`func NewPackageWithDefaults() *Package`

NewPackageWithDefaults instantiates a new Package object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Package) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Package) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Package) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *Package) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Package) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Package) SetId(v string)`

SetId sets Id field to given value.


### GetLookupKey

`func (o *Package) GetLookupKey() string`

GetLookupKey returns the LookupKey field if non-nil, zero value otherwise.

### GetLookupKeyOk

`func (o *Package) GetLookupKeyOk() (*string, bool)`

GetLookupKeyOk returns a tuple with the LookupKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLookupKey

`func (o *Package) SetLookupKey(v string)`

SetLookupKey sets LookupKey field to given value.


### GetDisplayName

`func (o *Package) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *Package) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *Package) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetPosition

`func (o *Package) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *Package) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *Package) SetPosition(v int32)`

SetPosition sets Position field to given value.


### SetPositionNil

`func (o *Package) SetPositionNil(b bool)`

 SetPositionNil sets the value for Position to be an explicit nil

### UnsetPosition
`func (o *Package) UnsetPosition()`

UnsetPosition ensures that no value is present for Position, not even an explicit nil
### GetCreatedAt

`func (o *Package) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Package) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Package) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.


### GetProducts

`func (o *Package) GetProducts() ProductList`

GetProducts returns the Products field if non-nil, zero value otherwise.

### GetProductsOk

`func (o *Package) GetProductsOk() (*ProductList, bool)`

GetProductsOk returns a tuple with the Products field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProducts

`func (o *Package) SetProducts(v ProductList)`

SetProducts sets Products field to given value.

### HasProducts

`func (o *Package) HasProducts() bool`

HasProducts returns a boolean if a field has been set.

### SetProductsNil

`func (o *Package) SetProductsNil(b bool)`

 SetProductsNil sets the value for Products to be an explicit nil

### UnsetProducts
`func (o *Package) UnsetProducts()`

UnsetProducts ensures that no value is present for Products, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


