# TransferCustomerDataRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TargetCustomerId** | **string** | The ID of the customer to whom the subscriptions and one-time purchases will be transferred. | 
**AppIds** | Pointer to **[]string** | Optional. The IDs of the apps to filter the transfer by. When specified, only purchases and subscriptions associated with these apps will be transferred. | [optional] 

## Methods

### NewTransferCustomerDataRequest

`func NewTransferCustomerDataRequest(targetCustomerId string, ) *TransferCustomerDataRequest`

NewTransferCustomerDataRequest instantiates a new TransferCustomerDataRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTransferCustomerDataRequestWithDefaults

`func NewTransferCustomerDataRequestWithDefaults() *TransferCustomerDataRequest`

NewTransferCustomerDataRequestWithDefaults instantiates a new TransferCustomerDataRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTargetCustomerId

`func (o *TransferCustomerDataRequest) GetTargetCustomerId() string`

GetTargetCustomerId returns the TargetCustomerId field if non-nil, zero value otherwise.

### GetTargetCustomerIdOk

`func (o *TransferCustomerDataRequest) GetTargetCustomerIdOk() (*string, bool)`

GetTargetCustomerIdOk returns a tuple with the TargetCustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetCustomerId

`func (o *TransferCustomerDataRequest) SetTargetCustomerId(v string)`

SetTargetCustomerId sets TargetCustomerId field to given value.


### GetAppIds

`func (o *TransferCustomerDataRequest) GetAppIds() []string`

GetAppIds returns the AppIds field if non-nil, zero value otherwise.

### GetAppIdsOk

`func (o *TransferCustomerDataRequest) GetAppIdsOk() (*[]string, bool)`

GetAppIdsOk returns a tuple with the AppIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppIds

`func (o *TransferCustomerDataRequest) SetAppIds(v []string)`

SetAppIds sets AppIds field to given value.

### HasAppIds

`func (o *TransferCustomerDataRequest) HasAppIds() bool`

HasAppIds returns a boolean if a field has been set.

### SetAppIdsNil

`func (o *TransferCustomerDataRequest) SetAppIdsNil(b bool)`

 SetAppIdsNil sets the value for AppIds to be an explicit nil

### UnsetAppIds
`func (o *TransferCustomerDataRequest) UnsetAppIds()`

UnsetAppIds ensures that no value is present for AppIds, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


