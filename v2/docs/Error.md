# Error

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Type** | **string** | The error type | 
**Param** | Pointer to **NullableString** | If the error is parameter-specific, the parameter related to the error | [optional] 
**DocUrl** | Pointer to **string** | A URL to more information about the error reported | [optional] 
**Message** | **string** | A message describing the reason of the error | 
**Retryable** | **bool** | Indicates if the error is retryable or not | 
**BackoffMs** | Pointer to **NullableInt32** | The ms the client should wait before retrying the request. Only present for retryable errors. | [optional] 

## Methods

### NewError

`func NewError(object string, type_ string, message string, retryable bool, ) *Error`

NewError instantiates a new Error object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewErrorWithDefaults

`func NewErrorWithDefaults() *Error`

NewErrorWithDefaults instantiates a new Error object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Error) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Error) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Error) SetObject(v string)`

SetObject sets Object field to given value.


### GetType

`func (o *Error) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Error) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Error) SetType(v string)`

SetType sets Type field to given value.


### GetParam

`func (o *Error) GetParam() string`

GetParam returns the Param field if non-nil, zero value otherwise.

### GetParamOk

`func (o *Error) GetParamOk() (*string, bool)`

GetParamOk returns a tuple with the Param field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParam

`func (o *Error) SetParam(v string)`

SetParam sets Param field to given value.

### HasParam

`func (o *Error) HasParam() bool`

HasParam returns a boolean if a field has been set.

### SetParamNil

`func (o *Error) SetParamNil(b bool)`

 SetParamNil sets the value for Param to be an explicit nil

### UnsetParam
`func (o *Error) UnsetParam()`

UnsetParam ensures that no value is present for Param, not even an explicit nil
### GetDocUrl

`func (o *Error) GetDocUrl() string`

GetDocUrl returns the DocUrl field if non-nil, zero value otherwise.

### GetDocUrlOk

`func (o *Error) GetDocUrlOk() (*string, bool)`

GetDocUrlOk returns a tuple with the DocUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDocUrl

`func (o *Error) SetDocUrl(v string)`

SetDocUrl sets DocUrl field to given value.

### HasDocUrl

`func (o *Error) HasDocUrl() bool`

HasDocUrl returns a boolean if a field has been set.

### GetMessage

`func (o *Error) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *Error) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *Error) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetRetryable

`func (o *Error) GetRetryable() bool`

GetRetryable returns the Retryable field if non-nil, zero value otherwise.

### GetRetryableOk

`func (o *Error) GetRetryableOk() (*bool, bool)`

GetRetryableOk returns a tuple with the Retryable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRetryable

`func (o *Error) SetRetryable(v bool)`

SetRetryable sets Retryable field to given value.


### GetBackoffMs

`func (o *Error) GetBackoffMs() int32`

GetBackoffMs returns the BackoffMs field if non-nil, zero value otherwise.

### GetBackoffMsOk

`func (o *Error) GetBackoffMsOk() (*int32, bool)`

GetBackoffMsOk returns a tuple with the BackoffMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBackoffMs

`func (o *Error) SetBackoffMs(v int32)`

SetBackoffMs sets BackoffMs field to given value.

### HasBackoffMs

`func (o *Error) HasBackoffMs() bool`

HasBackoffMs returns a boolean if a field has been set.

### SetBackoffMsNil

`func (o *Error) SetBackoffMsNil(b bool)`

 SetBackoffMsNil sets the value for BackoffMs to be an explicit nil

### UnsetBackoffMs
`func (o *Error) UnsetBackoffMs()`

UnsetBackoffMs ensures that no value is present for BackoffMs, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


