# UpdatePackageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DisplayName** | Pointer to **string** | The display name of the package | [optional] 
**Position** | Pointer to **int32** | The position of the package within the offering | [optional] 

## Methods

### NewUpdatePackageRequest

`func NewUpdatePackageRequest() *UpdatePackageRequest`

NewUpdatePackageRequest instantiates a new UpdatePackageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdatePackageRequestWithDefaults

`func NewUpdatePackageRequestWithDefaults() *UpdatePackageRequest`

NewUpdatePackageRequestWithDefaults instantiates a new UpdatePackageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDisplayName

`func (o *UpdatePackageRequest) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *UpdatePackageRequest) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *UpdatePackageRequest) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *UpdatePackageRequest) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### GetPosition

`func (o *UpdatePackageRequest) GetPosition() int32`

GetPosition returns the Position field if non-nil, zero value otherwise.

### GetPositionOk

`func (o *UpdatePackageRequest) GetPositionOk() (*int32, bool)`

GetPositionOk returns a tuple with the Position field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosition

`func (o *UpdatePackageRequest) SetPosition(v int32)`

SetPosition sets Position field to given value.

### HasPosition

`func (o *UpdatePackageRequest) HasPosition() bool`

HasPosition returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


