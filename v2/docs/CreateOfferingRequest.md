# CreateOfferingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LookupKey** | **string** | The custom identifier of the offering | 
**DisplayName** | **string** | The display_name of the offering | 
**Metadata** | Pointer to **map[string]interface{}** | Custom metadata of the offering | [optional] 

## Methods

### NewCreateOfferingRequest

`func NewCreateOfferingRequest(lookupKey string, displayName string, ) *CreateOfferingRequest`

NewCreateOfferingRequest instantiates a new CreateOfferingRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateOfferingRequestWithDefaults

`func NewCreateOfferingRequestWithDefaults() *CreateOfferingRequest`

NewCreateOfferingRequestWithDefaults instantiates a new CreateOfferingRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLookupKey

`func (o *CreateOfferingRequest) GetLookupKey() string`

GetLookupKey returns the LookupKey field if non-nil, zero value otherwise.

### GetLookupKeyOk

`func (o *CreateOfferingRequest) GetLookupKeyOk() (*string, bool)`

GetLookupKeyOk returns a tuple with the LookupKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLookupKey

`func (o *CreateOfferingRequest) SetLookupKey(v string)`

SetLookupKey sets LookupKey field to given value.


### GetDisplayName

`func (o *CreateOfferingRequest) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *CreateOfferingRequest) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *CreateOfferingRequest) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### GetMetadata

`func (o *CreateOfferingRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *CreateOfferingRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *CreateOfferingRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *CreateOfferingRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### SetMetadataNil

`func (o *CreateOfferingRequest) SetMetadataNil(b bool)`

 SetMetadataNil sets the value for Metadata to be an explicit nil

### UnsetMetadata
`func (o *CreateOfferingRequest) UnsetMetadata()`

UnsetMetadata ensures that no value is present for Metadata, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


