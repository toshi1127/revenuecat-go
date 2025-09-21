# CustomerAttribute

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Name** | **string** | The name of the attribute. Reserved attributes are prefixed with a &#x60;$&#x60;. | 
**Value** | **NullableString** | The value of the attribute. | 
**UpdatedAt** | **int64** | The time when the attribute was last updated. | 

## Methods

### NewCustomerAttribute

`func NewCustomerAttribute(object string, name string, value NullableString, updatedAt int64, ) *CustomerAttribute`

NewCustomerAttribute instantiates a new CustomerAttribute object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCustomerAttributeWithDefaults

`func NewCustomerAttributeWithDefaults() *CustomerAttribute`

NewCustomerAttributeWithDefaults instantiates a new CustomerAttribute object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *CustomerAttribute) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *CustomerAttribute) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *CustomerAttribute) SetObject(v string)`

SetObject sets Object field to given value.


### GetName

`func (o *CustomerAttribute) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CustomerAttribute) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CustomerAttribute) SetName(v string)`

SetName sets Name field to given value.


### GetValue

`func (o *CustomerAttribute) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *CustomerAttribute) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *CustomerAttribute) SetValue(v string)`

SetValue sets Value field to given value.


### SetValueNil

`func (o *CustomerAttribute) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *CustomerAttribute) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil
### GetUpdatedAt

`func (o *CustomerAttribute) GetUpdatedAt() int64`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *CustomerAttribute) GetUpdatedAtOk() (*int64, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *CustomerAttribute) SetUpdatedAt(v int64)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


