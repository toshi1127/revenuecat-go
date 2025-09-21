# SetCustomerAttributesRequestAttributesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | [**CreateCustomerRequestAttributesInnerName**](CreateCustomerRequestAttributesInnerName.md) |  | 
**Value** | **NullableString** | The value of the attribute. Use null to delete the attribute. | 

## Methods

### NewSetCustomerAttributesRequestAttributesInner

`func NewSetCustomerAttributesRequestAttributesInner(name CreateCustomerRequestAttributesInnerName, value NullableString, ) *SetCustomerAttributesRequestAttributesInner`

NewSetCustomerAttributesRequestAttributesInner instantiates a new SetCustomerAttributesRequestAttributesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSetCustomerAttributesRequestAttributesInnerWithDefaults

`func NewSetCustomerAttributesRequestAttributesInnerWithDefaults() *SetCustomerAttributesRequestAttributesInner`

NewSetCustomerAttributesRequestAttributesInnerWithDefaults instantiates a new SetCustomerAttributesRequestAttributesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *SetCustomerAttributesRequestAttributesInner) GetName() CreateCustomerRequestAttributesInnerName`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SetCustomerAttributesRequestAttributesInner) GetNameOk() (*CreateCustomerRequestAttributesInnerName, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SetCustomerAttributesRequestAttributesInner) SetName(v CreateCustomerRequestAttributesInnerName)`

SetName sets Name field to given value.


### GetValue

`func (o *SetCustomerAttributesRequestAttributesInner) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *SetCustomerAttributesRequestAttributesInner) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *SetCustomerAttributesRequestAttributesInner) SetValue(v string)`

SetValue sets Value field to given value.


### SetValueNil

`func (o *SetCustomerAttributesRequestAttributesInner) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *SetCustomerAttributesRequestAttributesInner) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


