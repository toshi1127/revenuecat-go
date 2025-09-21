# SubscriptionProduct

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Duration** | **NullableString** | The duration of the subscription in ISO-8601 standard | 
**GracePeriodDuration** | **NullableString** | The duration of the subscription&#39;s grace period in ISO-8601 standard | 
**TrialDuration** | **NullableString** | The duration of the subscription&#39;s trial period in ISO-8601 standard | 

## Methods

### NewSubscriptionProduct

`func NewSubscriptionProduct(duration NullableString, gracePeriodDuration NullableString, trialDuration NullableString, ) *SubscriptionProduct`

NewSubscriptionProduct instantiates a new SubscriptionProduct object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSubscriptionProductWithDefaults

`func NewSubscriptionProductWithDefaults() *SubscriptionProduct`

NewSubscriptionProductWithDefaults instantiates a new SubscriptionProduct object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDuration

`func (o *SubscriptionProduct) GetDuration() string`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *SubscriptionProduct) GetDurationOk() (*string, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *SubscriptionProduct) SetDuration(v string)`

SetDuration sets Duration field to given value.


### SetDurationNil

`func (o *SubscriptionProduct) SetDurationNil(b bool)`

 SetDurationNil sets the value for Duration to be an explicit nil

### UnsetDuration
`func (o *SubscriptionProduct) UnsetDuration()`

UnsetDuration ensures that no value is present for Duration, not even an explicit nil
### GetGracePeriodDuration

`func (o *SubscriptionProduct) GetGracePeriodDuration() string`

GetGracePeriodDuration returns the GracePeriodDuration field if non-nil, zero value otherwise.

### GetGracePeriodDurationOk

`func (o *SubscriptionProduct) GetGracePeriodDurationOk() (*string, bool)`

GetGracePeriodDurationOk returns a tuple with the GracePeriodDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGracePeriodDuration

`func (o *SubscriptionProduct) SetGracePeriodDuration(v string)`

SetGracePeriodDuration sets GracePeriodDuration field to given value.


### SetGracePeriodDurationNil

`func (o *SubscriptionProduct) SetGracePeriodDurationNil(b bool)`

 SetGracePeriodDurationNil sets the value for GracePeriodDuration to be an explicit nil

### UnsetGracePeriodDuration
`func (o *SubscriptionProduct) UnsetGracePeriodDuration()`

UnsetGracePeriodDuration ensures that no value is present for GracePeriodDuration, not even an explicit nil
### GetTrialDuration

`func (o *SubscriptionProduct) GetTrialDuration() string`

GetTrialDuration returns the TrialDuration field if non-nil, zero value otherwise.

### GetTrialDurationOk

`func (o *SubscriptionProduct) GetTrialDurationOk() (*string, bool)`

GetTrialDurationOk returns a tuple with the TrialDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialDuration

`func (o *SubscriptionProduct) SetTrialDuration(v string)`

SetTrialDuration sets TrialDuration field to given value.


### SetTrialDurationNil

`func (o *SubscriptionProduct) SetTrialDurationNil(b bool)`

 SetTrialDurationNil sets the value for TrialDuration to be an explicit nil

### UnsetTrialDuration
`func (o *SubscriptionProduct) UnsetTrialDuration()`

UnsetTrialDuration ensures that no value is present for TrialDuration, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


