# UpdateAppRequestAmazon

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PackageName** | Pointer to **string** | The package name of the app | [optional] 
**SharedSecret** | Pointer to **NullableString** | Your Amazon Developer Identity Shared Key | [optional] 

## Methods

### NewUpdateAppRequestAmazon

`func NewUpdateAppRequestAmazon() *UpdateAppRequestAmazon`

NewUpdateAppRequestAmazon instantiates a new UpdateAppRequestAmazon object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAppRequestAmazonWithDefaults

`func NewUpdateAppRequestAmazonWithDefaults() *UpdateAppRequestAmazon`

NewUpdateAppRequestAmazonWithDefaults instantiates a new UpdateAppRequestAmazon object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPackageName

`func (o *UpdateAppRequestAmazon) GetPackageName() string`

GetPackageName returns the PackageName field if non-nil, zero value otherwise.

### GetPackageNameOk

`func (o *UpdateAppRequestAmazon) GetPackageNameOk() (*string, bool)`

GetPackageNameOk returns a tuple with the PackageName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackageName

`func (o *UpdateAppRequestAmazon) SetPackageName(v string)`

SetPackageName sets PackageName field to given value.

### HasPackageName

`func (o *UpdateAppRequestAmazon) HasPackageName() bool`

HasPackageName returns a boolean if a field has been set.

### GetSharedSecret

`func (o *UpdateAppRequestAmazon) GetSharedSecret() string`

GetSharedSecret returns the SharedSecret field if non-nil, zero value otherwise.

### GetSharedSecretOk

`func (o *UpdateAppRequestAmazon) GetSharedSecretOk() (*string, bool)`

GetSharedSecretOk returns a tuple with the SharedSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSharedSecret

`func (o *UpdateAppRequestAmazon) SetSharedSecret(v string)`

SetSharedSecret sets SharedSecret field to given value.

### HasSharedSecret

`func (o *UpdateAppRequestAmazon) HasSharedSecret() bool`

HasSharedSecret returns a boolean if a field has been set.

### SetSharedSecretNil

`func (o *UpdateAppRequestAmazon) SetSharedSecretNil(b bool)`

 SetSharedSecretNil sets the value for SharedSecret to be an explicit nil

### UnsetSharedSecret
`func (o *UpdateAppRequestAmazon) UnsetSharedSecret()`

UnsetSharedSecret ensures that no value is present for SharedSecret, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


