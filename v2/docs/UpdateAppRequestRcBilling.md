# UpdateAppRequestRcBilling

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StripeAccountId** | Pointer to **NullableString** | It needs to be connected to your RevenueCat account. It can be omitted if you only have a single Stripe account connected to your RevenueCat account. | [optional] 
**AppName** | Pointer to **NullableString** | Shown in checkout, emails, and receipts sent to customers. | [optional] 
**SupportEmail** | Pointer to **NullableString** | Used as the &#x60;reply to&#x60; address in all emails sent to customers, to allow them to receive support. If you leave this field blank, your RevenueCat account email address will be used. | [optional] 
**DefaultCurrency** | Pointer to [**RCBillingCurrency**](RCBillingCurrency.md) |  | [optional] 

## Methods

### NewUpdateAppRequestRcBilling

`func NewUpdateAppRequestRcBilling() *UpdateAppRequestRcBilling`

NewUpdateAppRequestRcBilling instantiates a new UpdateAppRequestRcBilling object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAppRequestRcBillingWithDefaults

`func NewUpdateAppRequestRcBillingWithDefaults() *UpdateAppRequestRcBilling`

NewUpdateAppRequestRcBillingWithDefaults instantiates a new UpdateAppRequestRcBilling object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStripeAccountId

`func (o *UpdateAppRequestRcBilling) GetStripeAccountId() string`

GetStripeAccountId returns the StripeAccountId field if non-nil, zero value otherwise.

### GetStripeAccountIdOk

`func (o *UpdateAppRequestRcBilling) GetStripeAccountIdOk() (*string, bool)`

GetStripeAccountIdOk returns a tuple with the StripeAccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripeAccountId

`func (o *UpdateAppRequestRcBilling) SetStripeAccountId(v string)`

SetStripeAccountId sets StripeAccountId field to given value.

### HasStripeAccountId

`func (o *UpdateAppRequestRcBilling) HasStripeAccountId() bool`

HasStripeAccountId returns a boolean if a field has been set.

### SetStripeAccountIdNil

`func (o *UpdateAppRequestRcBilling) SetStripeAccountIdNil(b bool)`

 SetStripeAccountIdNil sets the value for StripeAccountId to be an explicit nil

### UnsetStripeAccountId
`func (o *UpdateAppRequestRcBilling) UnsetStripeAccountId()`

UnsetStripeAccountId ensures that no value is present for StripeAccountId, not even an explicit nil
### GetAppName

`func (o *UpdateAppRequestRcBilling) GetAppName() string`

GetAppName returns the AppName field if non-nil, zero value otherwise.

### GetAppNameOk

`func (o *UpdateAppRequestRcBilling) GetAppNameOk() (*string, bool)`

GetAppNameOk returns a tuple with the AppName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppName

`func (o *UpdateAppRequestRcBilling) SetAppName(v string)`

SetAppName sets AppName field to given value.

### HasAppName

`func (o *UpdateAppRequestRcBilling) HasAppName() bool`

HasAppName returns a boolean if a field has been set.

### SetAppNameNil

`func (o *UpdateAppRequestRcBilling) SetAppNameNil(b bool)`

 SetAppNameNil sets the value for AppName to be an explicit nil

### UnsetAppName
`func (o *UpdateAppRequestRcBilling) UnsetAppName()`

UnsetAppName ensures that no value is present for AppName, not even an explicit nil
### GetSupportEmail

`func (o *UpdateAppRequestRcBilling) GetSupportEmail() string`

GetSupportEmail returns the SupportEmail field if non-nil, zero value otherwise.

### GetSupportEmailOk

`func (o *UpdateAppRequestRcBilling) GetSupportEmailOk() (*string, bool)`

GetSupportEmailOk returns a tuple with the SupportEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportEmail

`func (o *UpdateAppRequestRcBilling) SetSupportEmail(v string)`

SetSupportEmail sets SupportEmail field to given value.

### HasSupportEmail

`func (o *UpdateAppRequestRcBilling) HasSupportEmail() bool`

HasSupportEmail returns a boolean if a field has been set.

### SetSupportEmailNil

`func (o *UpdateAppRequestRcBilling) SetSupportEmailNil(b bool)`

 SetSupportEmailNil sets the value for SupportEmail to be an explicit nil

### UnsetSupportEmail
`func (o *UpdateAppRequestRcBilling) UnsetSupportEmail()`

UnsetSupportEmail ensures that no value is present for SupportEmail, not even an explicit nil
### GetDefaultCurrency

`func (o *UpdateAppRequestRcBilling) GetDefaultCurrency() RCBillingCurrency`

GetDefaultCurrency returns the DefaultCurrency field if non-nil, zero value otherwise.

### GetDefaultCurrencyOk

`func (o *UpdateAppRequestRcBilling) GetDefaultCurrencyOk() (*RCBillingCurrency, bool)`

GetDefaultCurrencyOk returns a tuple with the DefaultCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCurrency

`func (o *UpdateAppRequestRcBilling) SetDefaultCurrency(v RCBillingCurrency)`

SetDefaultCurrency sets DefaultCurrency field to given value.

### HasDefaultCurrency

`func (o *UpdateAppRequestRcBilling) HasDefaultCurrency() bool`

HasDefaultCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


