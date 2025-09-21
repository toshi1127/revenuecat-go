# Offering

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The id of the offering | 
**LookupKey** | **string** | A custom identifier of the entitlement | 
**DisplayName** | **string** | The display name of the offering | 
**IsCurrent** | **bool** | Indicates if the offering is the current offering | 
**CreatedAt** | **int64** | The date the offering was created at in ms since epoch | 
**ProjectId** | **string** | ID of the project to which the offering belongs | 
**Metadata** | Pointer to **map[string]interface{}** | Custom metadata of the offering | [optional] 
**Packages** | Pointer to [**NullablePackageList**](PackageList.md) |  | [optional] 

## Methods

### NewOffering

`func NewOffering(object string, id string, lookupKey string, displayName string, isCurrent bool, createdAt int64, projectId string, ) *Offering`

NewOffering instantiates a new Offering object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOfferingWithDefaults

`func NewOfferingWithDefaults() *Offering`

NewOfferingWithDefaults instantiates a new Offering object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Offering) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Offering) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Offering) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *Offering) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Offering) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Offering) SetId(v string)`

SetId sets Id field to given value.


### GetLookupKey

`func (o *Offering) GetLookupKey() string`

GetLookupKey returns the LookupKey field if non-nil, zero value otherwise.

### GetLookupKeyOk

`func (o *Offering) GetLookupKeyOk() (*string, bool)`

GetLookupKeyOk returns a tuple with the LookupKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLookupKey

`func (o *Offering) SetLookupKey(v string)`

SetLookupKey sets LookupKey field to given value.


### GetDisplayName

`func (o *Offering) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *Offering) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *Offering) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetIsCurrent

`func (o *Offering) GetIsCurrent() bool`

GetIsCurrent returns the IsCurrent field if non-nil, zero value otherwise.

### GetIsCurrentOk

`func (o *Offering) GetIsCurrentOk() (*bool, bool)`

GetIsCurrentOk returns a tuple with the IsCurrent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCurrent

`func (o *Offering) SetIsCurrent(v bool)`

SetIsCurrent sets IsCurrent field to given value.


### GetCreatedAt

`func (o *Offering) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Offering) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Offering) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.


### GetProjectId

`func (o *Offering) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *Offering) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *Offering) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.


### GetMetadata

`func (o *Offering) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *Offering) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *Offering) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *Offering) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### SetMetadataNil

`func (o *Offering) SetMetadataNil(b bool)`

 SetMetadataNil sets the value for Metadata to be an explicit nil

### UnsetMetadata
`func (o *Offering) UnsetMetadata()`

UnsetMetadata ensures that no value is present for Metadata, not even an explicit nil
### GetPackages

`func (o *Offering) GetPackages() PackageList`

GetPackages returns the Packages field if non-nil, zero value otherwise.

### GetPackagesOk

`func (o *Offering) GetPackagesOk() (*PackageList, bool)`

GetPackagesOk returns a tuple with the Packages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackages

`func (o *Offering) SetPackages(v PackageList)`

SetPackages sets Packages field to given value.

### HasPackages

`func (o *Offering) HasPackages() bool`

HasPackages returns a boolean if a field has been set.

### SetPackagesNil

`func (o *Offering) SetPackagesNil(b bool)`

 SetPackagesNil sets the value for Packages to be an explicit nil

### UnsetPackages
`func (o *Offering) UnsetPackages()`

UnsetPackages ensures that no value is present for Packages, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


