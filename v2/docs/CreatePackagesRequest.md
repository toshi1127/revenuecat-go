# CreatePackagesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LookupKey** | **string** | The lookup_key of the package | 
**DisplayName** | **string** | The display name of the package | 
**Position** | Pointer to **int32** | The position of the package in the offering | [optional] 

## Methods

### NewCreatePackagesRequest

`func NewCreatePackagesRequest(lookupKey string, displayName string, ) *CreatePackagesRequest`

NewCreatePackagesRequest instantiates a new CreatePackagesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePackagesRequestWithDefaults

`func NewCreatePackagesRequestWithDefaults() *CreatePackagesRequest`

NewCreatePackagesRequestWithDefaults instantiates a new CreatePackagesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLookupKey

`func (o *CreatePackagesRequest) GetLookupKey() string`

GetLookupKey returns the LookupKey field if non-nil, zero value otherwise.

### GetLookupKeyOk

`func (o *CreatePackagesRequest) GetLookupKeyOk() (*string, bool)`

GetLookupKeyOk returns a tuple with the LookupKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLookupKey

`func (o *CreatePackagesRequest) SetLookupKey(v string)`

SetLookupKey sets LookupKey field to given value.


### GetDisplayName

`func (o *CreatePackagesRequest) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *CreatePackagesRequest) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *CreatePackagesRequest) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetPosition

`func (o *CreatePackagesRequest) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *CreatePackagesRequest) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *CreatePackagesRequest) SetPosition(v int32)`

SetPosition sets Position field to given value.

### HasPosition

`func (o *CreatePackagesRequest) HasPosition() bool`

HasPosition returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


