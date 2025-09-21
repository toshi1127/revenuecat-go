# RCBillingAppCreateRcBilling

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StripeAccountId** | Pointer to **NullableString** | It needs to be connected to your RevenueCat account. It can be omitted if you only have a single Stripe account connected to your RevenueCat account. | [optional] 
**AppName** | **string** | Shown in checkout, emails, and receipts sent to customers. | 
**SupportEmail** | Pointer to **NullableString** | Used as the &#x60;reply to&#x60; address in all emails sent to customers, to allow them to receive support.  If you leave this field blank, your RevenueCat account email address will be used. | [optional] 
**DefaultCurrency** | Pointer to [**RCBillingCurrency**](RCBillingCurrency.md) |  | [optional] 

## Methods

### NewRCBillingAppCreateRcBilling

`func NewRCBillingAppCreateRcBilling(appName string, ) *RCBillingAppCreateRcBilling`

NewRCBillingAppCreateRcBilling instantiates a new RCBillingAppCreateRcBilling object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRCBillingAppCreateRcBillingWithDefaults

`func NewRCBillingAppCreateRcBillingWithDefaults() *RCBillingAppCreateRcBilling`

NewRCBillingAppCreateRcBillingWithDefaults instantiates a new RCBillingAppCreateRcBilling object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStripeAccountId

`func (o *RCBillingAppCreateRcBilling) GetStripeAccountId() string`

GetStripeAccountId returns the StripeAccountId field if non-nil, zero value otherwise.

### GetStripeAccountIdOk

`func (o *RCBillingAppCreateRcBilling) GetStripeAccountIdOk() (*string, bool)`

GetStripeAccountIdOk returns a tuple with the StripeAccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripeAccountId

`func (o *RCBillingAppCreateRcBilling) SetStripeAccountId(v string)`

SetStripeAccountId sets StripeAccountId field to given value.

### HasStripeAccountId

`func (o *RCBillingAppCreateRcBilling) HasStripeAccountId() bool`

HasStripeAccountId returns a boolean if a field has been set.

### SetStripeAccountIdNil

`func (o *RCBillingAppCreateRcBilling) SetStripeAccountIdNil(b bool)`

 SetStripeAccountIdNil sets the value for StripeAccountId to be an explicit nil

### UnsetStripeAccountId
`func (o *RCBillingAppCreateRcBilling) UnsetStripeAccountId()`

UnsetStripeAccountId ensures that no value is present for StripeAccountId, not even an explicit nil
### GetAppName

`func (o *RCBillingAppCreateRcBilling) GetAppName() string`

GetAppName returns the AppName field if non-nil, zero value otherwise.

### GetAppNameOk

`func (o *RCBillingAppCreateRcBilling) GetAppNameOk() (*string, bool)`

GetAppNameOk returns a tuple with the AppName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppName

`func (o *RCBillingAppCreateRcBilling) SetAppName(v string)`

SetAppName sets AppName field to given value.


### GetSupportEmail

`func (o *RCBillingAppCreateRcBilling) GetSupportEmail() string`

GetSupportEmail returns the SupportEmail field if non-nil, zero value otherwise.

### GetSupportEmailOk

`func (o *RCBillingAppCreateRcBilling) GetSupportEmailOk() (*string, bool)`

GetSupportEmailOk returns a tuple with the SupportEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportEmail

`func (o *RCBillingAppCreateRcBilling) SetSupportEmail(v string)`

SetSupportEmail sets SupportEmail field to given value.

### HasSupportEmail

`func (o *RCBillingAppCreateRcBilling) HasSupportEmail() bool`

HasSupportEmail returns a boolean if a field has been set.

### SetSupportEmailNil

`func (o *RCBillingAppCreateRcBilling) SetSupportEmailNil(b bool)`

 SetSupportEmailNil sets the value for SupportEmail to be an explicit nil

### UnsetSupportEmail
`func (o *RCBillingAppCreateRcBilling) UnsetSupportEmail()`

UnsetSupportEmail ensures that no value is present for SupportEmail, not even an explicit nil
### GetDefaultCurrency

`func (o *RCBillingAppCreateRcBilling) GetDefaultCurrency() RCBillingCurrency`

GetDefaultCurrency returns the DefaultCurrency field if non-nil, zero value otherwise.

### GetDefaultCurrencyOk

`func (o *RCBillingAppCreateRcBilling) GetDefaultCurrencyOk() (*RCBillingCurrency, bool)`

GetDefaultCurrencyOk returns a tuple with the DefaultCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCurrency

`func (o *RCBillingAppCreateRcBilling) SetDefaultCurrency(v RCBillingCurrency)`

SetDefaultCurrency sets DefaultCurrency field to given value.

### HasDefaultCurrency

`func (o *RCBillingAppCreateRcBilling) HasDefaultCurrency() bool`

HasDefaultCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


