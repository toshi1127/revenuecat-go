# PublicApiKey

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The ID of the public API key | 
**Key** | **string** | The value of the public API key | 
**Environment** | **string** | The environment the public API key is for | 
**AppId** | **string** | The ID of the app the public API key is for | 
**CreatedAt** | **int64** | The date when the public API key was created in ms since epoch | 

## Methods

### NewPublicApiKey

`func NewPublicApiKey(object string, id string, key string, environment string, appId string, createdAt int64, ) *PublicApiKey`

NewPublicApiKey instantiates a new PublicApiKey object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPublicApiKeyWithDefaults

`func NewPublicApiKeyWithDefaults() *PublicApiKey`

NewPublicApiKeyWithDefaults instantiates a new PublicApiKey object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *PublicApiKey) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *PublicApiKey) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *PublicApiKey) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *PublicApiKey) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PublicApiKey) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PublicApiKey) SetId(v string)`

SetId sets Id field to given value.


### GetKey

`func (o *PublicApiKey) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *PublicApiKey) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *PublicApiKey) SetKey(v string)`

SetKey sets Key field to given value.


### GetEnvironment

`func (o *PublicApiKey) GetEnvironment() string`

GetEnvironment returns the Environment field if non-nil, zero value otherwise.

### GetEnvironmentOk

`func (o *PublicApiKey) GetEnvironmentOk() (*string, bool)`

GetEnvironmentOk returns a tuple with the Environment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironment

`func (o *PublicApiKey) SetEnvironment(v string)`

SetEnvironment sets Environment field to given value.


### GetAppId

`func (o *PublicApiKey) GetAppId() string`

GetAppId returns the AppId field if non-nil, zero value otherwise.

### GetAppIdOk

`func (o *PublicApiKey) GetAppIdOk() (*string, bool)`

GetAppIdOk returns a tuple with the AppId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppId

`func (o *PublicApiKey) SetAppId(v string)`

SetAppId sets AppId field to given value.


### GetCreatedAt

`func (o *PublicApiKey) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *PublicApiKey) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *PublicApiKey) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


