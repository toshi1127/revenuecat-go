# Transfer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SourceCustomer** | [**Customer**](Customer.md) |  | 
**TargetCustomer** | [**Customer**](Customer.md) |  | 

## Methods

### NewTransfer

`func NewTransfer(sourceCustomer Customer, targetCustomer Customer, ) *Transfer`

NewTransfer instantiates a new Transfer object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTransferWithDefaults

`func NewTransferWithDefaults() *Transfer`

NewTransferWithDefaults instantiates a new Transfer object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSourceCustomer

`func (o *Transfer) GetSourceCustomer() Customer`

GetSourceCustomer returns the SourceCustomer field if non-nil, zero value otherwise.

### GetSourceCustomerOk

`func (o *Transfer) GetSourceCustomerOk() (*Customer, bool)`

GetSourceCustomerOk returns a tuple with the SourceCustomer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceCustomer

`func (o *Transfer) SetSourceCustomer(v Customer)`

SetSourceCustomer sets SourceCustomer field to given value.


### GetTargetCustomer

`func (o *Transfer) GetTargetCustomer() Customer`

GetTargetCustomer returns the TargetCustomer field if non-nil, zero value otherwise.

### GetTargetCustomerOk

`func (o *Transfer) GetTargetCustomerOk() (*Customer, bool)`

GetTargetCustomerOk returns a tuple with the TargetCustomer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetCustomer

`func (o *Transfer) SetTargetCustomer(v Customer)`

SetTargetCustomer sets TargetCustomer field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


