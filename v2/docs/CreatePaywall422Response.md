# CreatePaywall422Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Type** | **string** |  | 
**Param** | Pointer to **NullableString** | If the error is parameter-specific, the parameter related to the error | [optional] 
**DocUrl** | Pointer to **string** | A URL to more information about the error reported | [optional] 
**Message** | **string** | A message describing the reason of the error | 
**Retryable** | **bool** | Indicates if the error is retryable or not | 
**BackoffMs** | Pointer to **NullableInt32** | The ms the client should wait before retrying the request. Only present for retryable errors. | [optional] 

## Methods

### NewCreatePaywall422Response

`func NewCreatePaywall422Response(object string, type_ string, message string, retryable bool, ) *CreatePaywall422Response`

NewCreatePaywall422Response instantiates a new CreatePaywall422Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePaywall422ResponseWithDefaults

`func NewCreatePaywall422ResponseWithDefaults() *CreatePaywall422Response`

NewCreatePaywall422ResponseWithDefaults instantiates a new CreatePaywall422Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *CreatePaywall422Response) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *CreatePaywall422Response) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *CreatePaywall422Response) SetObject(v string)`

SetObject sets Object field to given value.


### GetType

`func (o *CreatePaywall422Response) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreatePaywall422Response) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreatePaywall422Response) SetType(v string)`

SetType sets Type field to given value.


### GetParam

`func (o *CreatePaywall422Response) GetParam() string`

GetParam returns the Param field if non-nil, zero value otherwise.

### GetParamOk

`func (o *CreatePaywall422Response) GetParamOk() (*string, bool)`

GetParamOk returns a tuple with the Param field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParam

`func (o *CreatePaywall422Response) SetParam(v string)`

SetParam sets Param field to given value.

### HasParam

`func (o *CreatePaywall422Response) HasParam() bool`

HasParam returns a boolean if a field has been set.

### SetParamNil

`func (o *CreatePaywall422Response) SetParamNil(b bool)`

 SetParamNil sets the value for Param to be an explicit nil

### UnsetParam
`func (o *CreatePaywall422Response) UnsetParam()`

UnsetParam ensures that no value is present for Param, not even an explicit nil
### GetDocUrl

`func (o *CreatePaywall422Response) GetDocUrl() string`

GetDocUrl returns the DocUrl field if non-nil, zero value otherwise.

### GetDocUrlOk

`func (o *CreatePaywall422Response) GetDocUrlOk() (*string, bool)`

GetDocUrlOk returns a tuple with the DocUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocUrl

`func (o *CreatePaywall422Response) SetDocUrl(v string)`

SetDocUrl sets DocUrl field to given value.

### HasDocUrl

`func (o *CreatePaywall422Response) HasDocUrl() bool`

HasDocUrl returns a boolean if a field has been set.

### GetMessage

`func (o *CreatePaywall422Response) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *CreatePaywall422Response) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *CreatePaywall422Response) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetRetryable

`func (o *CreatePaywall422Response) GetRetryable() bool`

GetRetryable returns the Retryable field if non-nil, zero value otherwise.

### GetRetryableOk

`func (o *CreatePaywall422Response) GetRetryableOk() (*bool, bool)`

GetRetryableOk returns a tuple with the Retryable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRetryable

`func (o *CreatePaywall422Response) SetRetryable(v bool)`

SetRetryable sets Retryable field to given value.


### GetBackoffMs

`func (o *CreatePaywall422Response) GetBackoffMs() int32`

GetBackoffMs returns the BackoffMs field if non-nil, zero value otherwise.

### GetBackoffMsOk

`func (o *CreatePaywall422Response) GetBackoffMsOk() (*int32, bool)`

GetBackoffMsOk returns a tuple with the BackoffMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackoffMs

`func (o *CreatePaywall422Response) SetBackoffMs(v int32)`

SetBackoffMs sets BackoffMs field to given value.

### HasBackoffMs

`func (o *CreatePaywall422Response) HasBackoffMs() bool`

HasBackoffMs returns a boolean if a field has been set.

### SetBackoffMsNil

`func (o *CreatePaywall422Response) SetBackoffMsNil(b bool)`

 SetBackoffMsNil sets the value for BackoffMs to be an explicit nil

### UnsetBackoffMs
`func (o *CreatePaywall422Response) UnsetBackoffMs()`

UnsetBackoffMs ensures that no value is present for BackoffMs, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


