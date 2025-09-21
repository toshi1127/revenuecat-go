# PaddleAppCreatePaddle

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PaddleApiKey** | Pointer to **NullableString** | Paddle Server-side API key provided on the Paddle dashboard. | [optional] 
**PaddleIsSandbox** | Pointer to **NullableBool** | [Deprecated] Whether the app is tied to the sandbox environment. This field is deprecated and will be removed in the future. The environment is determined by the &#x60;paddle_api_key&#x60; format.  | [optional] 

## Methods

### NewPaddleAppCreatePaddle

`func NewPaddleAppCreatePaddle() *PaddleAppCreatePaddle`

NewPaddleAppCreatePaddle instantiates a new PaddleAppCreatePaddle object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaddleAppCreatePaddleWithDefaults

`func NewPaddleAppCreatePaddleWithDefaults() *PaddleAppCreatePaddle`

NewPaddleAppCreatePaddleWithDefaults instantiates a new PaddleAppCreatePaddle object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPaddleApiKey

`func (o *PaddleAppCreatePaddle) GetPaddleApiKey() string`

GetPaddleApiKey returns the PaddleApiKey field if non-nil, zero value otherwise.

### GetPaddleApiKeyOk

`func (o *PaddleAppCreatePaddle) GetPaddleApiKeyOk() (*string, bool)`

GetPaddleApiKeyOk returns a tuple with the PaddleApiKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaddleApiKey

`func (o *PaddleAppCreatePaddle) SetPaddleApiKey(v string)`

SetPaddleApiKey sets PaddleApiKey field to given value.

### HasPaddleApiKey

`func (o *PaddleAppCreatePaddle) HasPaddleApiKey() bool`

HasPaddleApiKey returns a boolean if a field has been set.

### SetPaddleApiKeyNil

`func (o *PaddleAppCreatePaddle) SetPaddleApiKeyNil(b bool)`

 SetPaddleApiKeyNil sets the value for PaddleApiKey to be an explicit nil

### UnsetPaddleApiKey
`func (o *PaddleAppCreatePaddle) UnsetPaddleApiKey()`

UnsetPaddleApiKey ensures that no value is present for PaddleApiKey, not even an explicit nil
### GetPaddleIsSandbox

`func (o *PaddleAppCreatePaddle) GetPaddleIsSandbox() bool`

GetPaddleIsSandbox returns the PaddleIsSandbox field if non-nil, zero value otherwise.

### GetPaddleIsSandboxOk

`func (o *PaddleAppCreatePaddle) GetPaddleIsSandboxOk() (*bool, bool)`

GetPaddleIsSandboxOk returns a tuple with the PaddleIsSandbox field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaddleIsSandbox

`func (o *PaddleAppCreatePaddle) SetPaddleIsSandbox(v bool)`

SetPaddleIsSandbox sets PaddleIsSandbox field to given value.

### HasPaddleIsSandbox

`func (o *PaddleAppCreatePaddle) HasPaddleIsSandbox() bool`

HasPaddleIsSandbox returns a boolean if a field has been set.

### SetPaddleIsSandboxNil

`func (o *PaddleAppCreatePaddle) SetPaddleIsSandboxNil(b bool)`

 SetPaddleIsSandboxNil sets the value for PaddleIsSandbox to be an explicit nil

### UnsetPaddleIsSandbox
`func (o *PaddleAppCreatePaddle) UnsetPaddleIsSandbox()`

UnsetPaddleIsSandbox ensures that no value is present for PaddleIsSandbox, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


