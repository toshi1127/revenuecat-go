# AmazonAppCreateAmazon

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PackageName** | **string** | The package name of the app | 
**SharedSecret** | Pointer to **string** | Your Amazon Developer Identity Shared Key | [optional] 

## Methods

### NewAmazonAppCreateAmazon

`func NewAmazonAppCreateAmazon(packageName string, ) *AmazonAppCreateAmazon`

NewAmazonAppCreateAmazon instantiates a new AmazonAppCreateAmazon object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAmazonAppCreateAmazonWithDefaults

`func NewAmazonAppCreateAmazonWithDefaults() *AmazonAppCreateAmazon`

NewAmazonAppCreateAmazonWithDefaults instantiates a new AmazonAppCreateAmazon object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPackageName

`func (o *AmazonAppCreateAmazon) GetPackageName() string`

GetPackageName returns the PackageName field if non-nil, zero value otherwise.

### GetPackageNameOk

`func (o *AmazonAppCreateAmazon) GetPackageNameOk() (*string, bool)`

GetPackageNameOk returns a tuple with the PackageName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackageName

`func (o *AmazonAppCreateAmazon) SetPackageName(v string)`

SetPackageName sets PackageName field to given value.


### GetSharedSecret

`func (o *AmazonAppCreateAmazon) GetSharedSecret() string`

GetSharedSecret returns the SharedSecret field if non-nil, zero value otherwise.

### GetSharedSecretOk

`func (o *AmazonAppCreateAmazon) GetSharedSecretOk() (*string, bool)`

GetSharedSecretOk returns a tuple with the SharedSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSharedSecret

`func (o *AmazonAppCreateAmazon) SetSharedSecret(v string)`

SetSharedSecret sets SharedSecret field to given value.

### HasSharedSecret

`func (o *AmazonAppCreateAmazon) HasSharedSecret() bool`

HasSharedSecret returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


