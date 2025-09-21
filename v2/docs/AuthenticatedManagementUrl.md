# AuthenticatedManagementUrl

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**ManagementUrl** | **string** | A secure, single-use URL that provides temporary access to the customer portal for a specific customer. This URL can only be used once and expires after use. | 

## Methods

### NewAuthenticatedManagementUrl

`func NewAuthenticatedManagementUrl(object string, managementUrl string, ) *AuthenticatedManagementUrl`

NewAuthenticatedManagementUrl instantiates a new AuthenticatedManagementUrl object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthenticatedManagementUrlWithDefaults

`func NewAuthenticatedManagementUrlWithDefaults() *AuthenticatedManagementUrl`

NewAuthenticatedManagementUrlWithDefaults instantiates a new AuthenticatedManagementUrl object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *AuthenticatedManagementUrl) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *AuthenticatedManagementUrl) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *AuthenticatedManagementUrl) SetObject(v string)`

SetObject sets Object field to given value.


### GetManagementUrl

`func (o *AuthenticatedManagementUrl) GetManagementUrl() string`

GetManagementUrl returns the ManagementUrl field if non-nil, zero value otherwise.

### GetManagementUrlOk

`func (o *AuthenticatedManagementUrl) GetManagementUrlOk() (*string, bool)`

GetManagementUrlOk returns a tuple with the ManagementUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManagementUrl

`func (o *AuthenticatedManagementUrl) SetManagementUrl(v string)`

SetManagementUrl sets ManagementUrl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


