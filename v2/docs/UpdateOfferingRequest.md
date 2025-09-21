# UpdateOfferingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DisplayName** | Pointer to **string** | The display name of the offering | [optional] 
**IsCurrent** | Pointer to **bool** | Indicates if the offering is the current offering | [optional] 
**Metadata** | Pointer to **map[string]interface{}** | Custom metadata of the offering | [optional] 

## Methods

### NewUpdateOfferingRequest

`func NewUpdateOfferingRequest() *UpdateOfferingRequest`

NewUpdateOfferingRequest instantiates a new UpdateOfferingRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateOfferingRequestWithDefaults

`func NewUpdateOfferingRequestWithDefaults() *UpdateOfferingRequest`

NewUpdateOfferingRequestWithDefaults instantiates a new UpdateOfferingRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDisplayName

`func (o *UpdateOfferingRequest) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *UpdateOfferingRequest) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *UpdateOfferingRequest) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *UpdateOfferingRequest) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### GetIsCurrent

`func (o *UpdateOfferingRequest) GetIsCurrent() bool`

GetIsCurrent returns the IsCurrent field if non-nil, zero value otherwise.

### GetIsCurrentOk

`func (o *UpdateOfferingRequest) GetIsCurrentOk() (*bool, bool)`

GetIsCurrentOk returns a tuple with the IsCurrent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsCurrent

`func (o *UpdateOfferingRequest) SetIsCurrent(v bool)`

SetIsCurrent sets IsCurrent field to given value.

### HasIsCurrent

`func (o *UpdateOfferingRequest) HasIsCurrent() bool`

HasIsCurrent returns a boolean if a field has been set.

### GetMetadata

`func (o *UpdateOfferingRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *UpdateOfferingRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *UpdateOfferingRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *UpdateOfferingRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### SetMetadataNil

`func (o *UpdateOfferingRequest) SetMetadataNil(b bool)`

 SetMetadataNil sets the value for Metadata to be an explicit nil

### UnsetMetadata
`func (o *UpdateOfferingRequest) UnsetMetadata()`

UnsetMetadata ensures that no value is present for Metadata, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


