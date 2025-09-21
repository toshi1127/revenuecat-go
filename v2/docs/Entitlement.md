# Entitlement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**ProjectId** | **string** | ID of the project to which the entitlement belongs | 
**Id** | **string** | The id of the entitlement | 
**LookupKey** | **string** | A custom identifier of the entitlement | 
**DisplayName** | **string** | The display name of the entitlement | 
**CreatedAt** | **int64** | The date when the entitlement was created in ms since epoch | 
**Products** | Pointer to [**NullableProductsList**](ProductsList.md) |  | [optional] 

## Methods

### NewEntitlement

`func NewEntitlement(object string, projectId string, id string, lookupKey string, displayName string, createdAt int64, ) *Entitlement`

NewEntitlement instantiates a new Entitlement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntitlementWithDefaults

`func NewEntitlementWithDefaults() *Entitlement`

NewEntitlementWithDefaults instantiates a new Entitlement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Entitlement) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Entitlement) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Entitlement) SetObject(v string)`

SetObject sets Object field to given value.


### GetProjectId

`func (o *Entitlement) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *Entitlement) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *Entitlement) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.


### GetId

`func (o *Entitlement) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Entitlement) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Entitlement) SetId(v string)`

SetId sets Id field to given value.


### GetLookupKey

`func (o *Entitlement) GetLookupKey() string`

GetLookupKey returns the LookupKey field if non-nil, zero value otherwise.

### GetLookupKeyOk

`func (o *Entitlement) GetLookupKeyOk() (*string, bool)`

GetLookupKeyOk returns a tuple with the LookupKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLookupKey

`func (o *Entitlement) SetLookupKey(v string)`

SetLookupKey sets LookupKey field to given value.


### GetDisplayName

`func (o *Entitlement) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *Entitlement) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *Entitlement) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetCreatedAt

`func (o *Entitlement) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Entitlement) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Entitlement) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.


### GetProducts

`func (o *Entitlement) GetProducts() ProductsList`

GetProducts returns the Products field if non-nil, zero value otherwise.

### GetProductsOk

`func (o *Entitlement) GetProductsOk() (*ProductsList, bool)`

GetProductsOk returns a tuple with the Products field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProducts

`func (o *Entitlement) SetProducts(v ProductsList)`

SetProducts sets Products field to given value.

### HasProducts

`func (o *Entitlement) HasProducts() bool`

HasProducts returns a boolean if a field has been set.

### SetProductsNil

`func (o *Entitlement) SetProductsNil(b bool)`

 SetProductsNil sets the value for Products to be an explicit nil

### UnsetProducts
`func (o *Entitlement) UnsetProducts()`

UnsetProducts ensures that no value is present for Products, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


