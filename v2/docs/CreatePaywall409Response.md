# CreatePaywall409Response

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

### NewCreatePaywall409Response

`func NewCreatePaywall409Response(object string, type_ string, message string, retryable bool, ) *CreatePaywall409Response`

NewCreatePaywall409Response instantiates a new CreatePaywall409Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePaywall409ResponseWithDefaults

`func NewCreatePaywall409ResponseWithDefaults() *CreatePaywall409Response`

NewCreatePaywall409ResponseWithDefaults instantiates a new CreatePaywall409Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *CreatePaywall409Response) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *CreatePaywall409Response) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *CreatePaywall409Response) SetObject(v string)`

SetObject sets Object field to given value.


### GetType

`func (o *CreatePaywall409Response) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreatePaywall409Response) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreatePaywall409Response) SetType(v string)`

SetType sets Type field to given value.


### GetParam

`func (o *CreatePaywall409Response) GetParam() string`

GetParam returns the Param field if non-nil, zero value otherwise.

### GetParamOk

`func (o *CreatePaywall409Response) GetParamOk() (*string, bool)`

GetParamOk returns a tuple with the Param field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParam

`func (o *CreatePaywall409Response) SetParam(v string)`

SetParam sets Param field to given value.

### HasParam

`func (o *CreatePaywall409Response) HasParam() bool`

HasParam returns a boolean if a field has been set.

### SetParamNil

`func (o *CreatePaywall409Response) SetParamNil(b bool)`

 SetParamNil sets the value for Param to be an explicit nil

### UnsetParam
`func (o *CreatePaywall409Response) UnsetParam()`

UnsetParam ensures that no value is present for Param, not even an explicit nil
### GetDocUrl

`func (o *CreatePaywall409Response) GetDocUrl() string`

GetDocUrl returns the DocUrl field if non-nil, zero value otherwise.

### GetDocUrlOk

`func (o *CreatePaywall409Response) GetDocUrlOk() (*string, bool)`

GetDocUrlOk returns a tuple with the DocUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocUrl

`func (o *CreatePaywall409Response) SetDocUrl(v string)`

SetDocUrl sets DocUrl field to given value.

### HasDocUrl

`func (o *CreatePaywall409Response) HasDocUrl() bool`

HasDocUrl returns a boolean if a field has been set.

### GetMessage

`func (o *CreatePaywall409Response) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *CreatePaywall409Response) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *CreatePaywall409Response) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetRetryable

`func (o *CreatePaywall409Response) GetRetryable() bool`

GetRetryable returns the Retryable field if non-nil, zero value otherwise.

### GetRetryableOk

`func (o *CreatePaywall409Response) GetRetryableOk() (*bool, bool)`

GetRetryableOk returns a tuple with the Retryable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRetryable

`func (o *CreatePaywall409Response) SetRetryable(v bool)`

SetRetryable sets Retryable field to given value.


### GetBackoffMs

`func (o *CreatePaywall409Response) GetBackoffMs() int32`

GetBackoffMs returns the BackoffMs field if non-nil, zero value otherwise.

### GetBackoffMsOk

`func (o *CreatePaywall409Response) GetBackoffMsOk() (*int32, bool)`

GetBackoffMsOk returns a tuple with the BackoffMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackoffMs

`func (o *CreatePaywall409Response) SetBackoffMs(v int32)`

SetBackoffMs sets BackoffMs field to given value.

### HasBackoffMs

`func (o *CreatePaywall409Response) HasBackoffMs() bool`

HasBackoffMs returns a boolean if a field has been set.

### SetBackoffMsNil

`func (o *CreatePaywall409Response) SetBackoffMsNil(b bool)`

 SetBackoffMsNil sets the value for BackoffMs to be an explicit nil

### UnsetBackoffMs
`func (o *CreatePaywall409Response) UnsetBackoffMs()`

UnsetBackoffMs ensures that no value is present for BackoffMs, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


