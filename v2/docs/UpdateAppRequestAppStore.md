# UpdateAppRequestAppStore

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BundleId** | Pointer to **string** | The bundle ID of the app | [optional] 
**SharedSecret** | Pointer to **NullableString** | The shared secret of the app | [optional] 

## Methods

### NewUpdateAppRequestAppStore

`func NewUpdateAppRequestAppStore() *UpdateAppRequestAppStore`

NewUpdateAppRequestAppStore instantiates a new UpdateAppRequestAppStore object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAppRequestAppStoreWithDefaults

`func NewUpdateAppRequestAppStoreWithDefaults() *UpdateAppRequestAppStore`

NewUpdateAppRequestAppStoreWithDefaults instantiates a new UpdateAppRequestAppStore object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBundleId

`func (o *UpdateAppRequestAppStore) GetBundleId() string`

GetBundleId returns the BundleId field if non-nil, zero value otherwise.

### GetBundleIdOk

`func (o *UpdateAppRequestAppStore) GetBundleIdOk() (*string, bool)`

GetBundleIdOk returns a tuple with the BundleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBundleId

`func (o *UpdateAppRequestAppStore) SetBundleId(v string)`

SetBundleId sets BundleId field to given value.

### HasBundleId

`func (o *UpdateAppRequestAppStore) HasBundleId() bool`

HasBundleId returns a boolean if a field has been set.

### GetSharedSecret

`func (o *UpdateAppRequestAppStore) GetSharedSecret() string`

GetSharedSecret returns the SharedSecret field if non-nil, zero value otherwise.

### GetSharedSecretOk

`func (o *UpdateAppRequestAppStore) GetSharedSecretOk() (*string, bool)`

GetSharedSecretOk returns a tuple with the SharedSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSharedSecret

`func (o *UpdateAppRequestAppStore) SetSharedSecret(v string)`

SetSharedSecret sets SharedSecret field to given value.

### HasSharedSecret

`func (o *UpdateAppRequestAppStore) HasSharedSecret() bool`

HasSharedSecret returns a boolean if a field has been set.

### SetSharedSecretNil

`func (o *UpdateAppRequestAppStore) SetSharedSecretNil(b bool)`

 SetSharedSecretNil sets the value for SharedSecret to be an explicit nil

### UnsetSharedSecret
`func (o *UpdateAppRequestAppStore) UnsetSharedSecret()`

UnsetSharedSecret ensures that no value is present for SharedSecret, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


