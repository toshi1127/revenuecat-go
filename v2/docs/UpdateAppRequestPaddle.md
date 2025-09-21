# UpdateAppRequestPaddle

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PaddleApiKey** | Pointer to **NullableString** | Paddle Server-side API key provided on the Paddle dashboard. | [optional] 
**PaddleIsSandbox** | Pointer to **bool** | Whether the app is tied to the sandbox environment. | [optional] 

## Methods

### NewUpdateAppRequestPaddle

`func NewUpdateAppRequestPaddle() *UpdateAppRequestPaddle`

NewUpdateAppRequestPaddle instantiates a new UpdateAppRequestPaddle object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAppRequestPaddleWithDefaults

`func NewUpdateAppRequestPaddleWithDefaults() *UpdateAppRequestPaddle`

NewUpdateAppRequestPaddleWithDefaults instantiates a new UpdateAppRequestPaddle object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPaddleApiKey

`func (o *UpdateAppRequestPaddle) GetPaddleApiKey() string`

GetPaddleApiKey returns the PaddleApiKey field if non-nil, zero value otherwise.

### GetPaddleApiKeyOk

`func (o *UpdateAppRequestPaddle) GetPaddleApiKeyOk() (*string, bool)`

GetPaddleApiKeyOk returns a tuple with the PaddleApiKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaddleApiKey

`func (o *UpdateAppRequestPaddle) SetPaddleApiKey(v string)`

SetPaddleApiKey sets PaddleApiKey field to given value.

### HasPaddleApiKey

`func (o *UpdateAppRequestPaddle) HasPaddleApiKey() bool`

HasPaddleApiKey returns a boolean if a field has been set.

### SetPaddleApiKeyNil

`func (o *UpdateAppRequestPaddle) SetPaddleApiKeyNil(b bool)`

 SetPaddleApiKeyNil sets the value for PaddleApiKey to be an explicit nil

### UnsetPaddleApiKey
`func (o *UpdateAppRequestPaddle) UnsetPaddleApiKey()`

UnsetPaddleApiKey ensures that no value is present for PaddleApiKey, not even an explicit nil
### GetPaddleIsSandbox

`func (o *UpdateAppRequestPaddle) GetPaddleIsSandbox() bool`

GetPaddleIsSandbox returns the PaddleIsSandbox field if non-nil, zero value otherwise.

### GetPaddleIsSandboxOk

`func (o *UpdateAppRequestPaddle) GetPaddleIsSandboxOk() (*bool, bool)`

GetPaddleIsSandboxOk returns a tuple with the PaddleIsSandbox field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaddleIsSandbox

`func (o *UpdateAppRequestPaddle) SetPaddleIsSandbox(v bool)`

SetPaddleIsSandbox sets PaddleIsSandbox field to given value.

### HasPaddleIsSandbox

`func (o *UpdateAppRequestPaddle) HasPaddleIsSandbox() bool`

HasPaddleIsSandbox returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


