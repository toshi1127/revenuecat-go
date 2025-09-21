# RCBillingAppRcBilling

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StripeAccountId** | Pointer to **NullableString** | Stripe account connected to your RevenueCat account. | [optional] 
**SellerCompanyName** | **string** | The company name.  This field is deprecated. Please, use &#x60;app_name&#x60; instead. | 
**AppName** | Pointer to **string** | Shown in checkout, emails, and receipts sent to customers. | [optional] 
**SellerCompanySupportEmail** | Pointer to **NullableString** | The company support email. This field is deprecated. Please, use &#x60;support_email&#x60; instead. | [optional] 
**SupportEmail** | Pointer to **NullableString** | Used as the &#x60;reply to&#x60; address in all emails sent to customers, to allow them to receive support.  | [optional] 
**DefaultCurrency** | [**RCBillingCurrency**](RCBillingCurrency.md) |  | 

## Methods

### NewRCBillingAppRcBilling

`func NewRCBillingAppRcBilling(sellerCompanyName string, defaultCurrency RCBillingCurrency, ) *RCBillingAppRcBilling`

NewRCBillingAppRcBilling instantiates a new RCBillingAppRcBilling object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRCBillingAppRcBillingWithDefaults

`func NewRCBillingAppRcBillingWithDefaults() *RCBillingAppRcBilling`

NewRCBillingAppRcBillingWithDefaults instantiates a new RCBillingAppRcBilling object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStripeAccountId

`func (o *RCBillingAppRcBilling) GetStripeAccountId() string`

GetStripeAccountId returns the StripeAccountId field if non-nil, zero value otherwise.

### GetStripeAccountIdOk

`func (o *RCBillingAppRcBilling) GetStripeAccountIdOk() (*string, bool)`

GetStripeAccountIdOk returns a tuple with the StripeAccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripeAccountId

`func (o *RCBillingAppRcBilling) SetStripeAccountId(v string)`

SetStripeAccountId sets StripeAccountId field to given value.

### HasStripeAccountId

`func (o *RCBillingAppRcBilling) HasStripeAccountId() bool`

HasStripeAccountId returns a boolean if a field has been set.

### SetStripeAccountIdNil

`func (o *RCBillingAppRcBilling) SetStripeAccountIdNil(b bool)`

 SetStripeAccountIdNil sets the value for StripeAccountId to be an explicit nil

### UnsetStripeAccountId
`func (o *RCBillingAppRcBilling) UnsetStripeAccountId()`

UnsetStripeAccountId ensures that no value is present for StripeAccountId, not even an explicit nil
### GetSellerCompanyName

`func (o *RCBillingAppRcBilling) GetSellerCompanyName() string`

GetSellerCompanyName returns the SellerCompanyName field if non-nil, zero value otherwise.

### GetSellerCompanyNameOk

`func (o *RCBillingAppRcBilling) GetSellerCompanyNameOk() (*string, bool)`

GetSellerCompanyNameOk returns a tuple with the SellerCompanyName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerCompanyName

`func (o *RCBillingAppRcBilling) SetSellerCompanyName(v string)`

SetSellerCompanyName sets SellerCompanyName field to given value.


### GetAppName

`func (o *RCBillingAppRcBilling) GetAppName() string`

GetAppName returns the AppName field if non-nil, zero value otherwise.

### GetAppNameOk

`func (o *RCBillingAppRcBilling) GetAppNameOk() (*string, bool)`

GetAppNameOk returns a tuple with the AppName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppName

`func (o *RCBillingAppRcBilling) SetAppName(v string)`

SetAppName sets AppName field to given value.

### HasAppName

`func (o *RCBillingAppRcBilling) HasAppName() bool`

HasAppName returns a boolean if a field has been set.

### GetSellerCompanySupportEmail

`func (o *RCBillingAppRcBilling) GetSellerCompanySupportEmail() string`

GetSellerCompanySupportEmail returns the SellerCompanySupportEmail field if non-nil, zero value otherwise.

### GetSellerCompanySupportEmailOk

`func (o *RCBillingAppRcBilling) GetSellerCompanySupportEmailOk() (*string, bool)`

GetSellerCompanySupportEmailOk returns a tuple with the SellerCompanySupportEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSellerCompanySupportEmail

`func (o *RCBillingAppRcBilling) SetSellerCompanySupportEmail(v string)`

SetSellerCompanySupportEmail sets SellerCompanySupportEmail field to given value.

### HasSellerCompanySupportEmail

`func (o *RCBillingAppRcBilling) HasSellerCompanySupportEmail() bool`

HasSellerCompanySupportEmail returns a boolean if a field has been set.

### SetSellerCompanySupportEmailNil

`func (o *RCBillingAppRcBilling) SetSellerCompanySupportEmailNil(b bool)`

 SetSellerCompanySupportEmailNil sets the value for SellerCompanySupportEmail to be an explicit nil

### UnsetSellerCompanySupportEmail
`func (o *RCBillingAppRcBilling) UnsetSellerCompanySupportEmail()`

UnsetSellerCompanySupportEmail ensures that no value is present for SellerCompanySupportEmail, not even an explicit nil
### GetSupportEmail

`func (o *RCBillingAppRcBilling) GetSupportEmail() string`

GetSupportEmail returns the SupportEmail field if non-nil, zero value otherwise.

### GetSupportEmailOk

`func (o *RCBillingAppRcBilling) GetSupportEmailOk() (*string, bool)`

GetSupportEmailOk returns a tuple with the SupportEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportEmail

`func (o *RCBillingAppRcBilling) SetSupportEmail(v string)`

SetSupportEmail sets SupportEmail field to given value.

### HasSupportEmail

`func (o *RCBillingAppRcBilling) HasSupportEmail() bool`

HasSupportEmail returns a boolean if a field has been set.

### SetSupportEmailNil

`func (o *RCBillingAppRcBilling) SetSupportEmailNil(b bool)`

 SetSupportEmailNil sets the value for SupportEmail to be an explicit nil

### UnsetSupportEmail
`func (o *RCBillingAppRcBilling) UnsetSupportEmail()`

UnsetSupportEmail ensures that no value is present for SupportEmail, not even an explicit nil
### GetDefaultCurrency

`func (o *RCBillingAppRcBilling) GetDefaultCurrency() RCBillingCurrency`

GetDefaultCurrency returns the DefaultCurrency field if non-nil, zero value otherwise.

### GetDefaultCurrencyOk

`func (o *RCBillingAppRcBilling) GetDefaultCurrencyOk() (*RCBillingCurrency, bool)`

GetDefaultCurrencyOk returns a tuple with the DefaultCurrency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCurrency

`func (o *RCBillingAppRcBilling) SetDefaultCurrency(v RCBillingCurrency)`

SetDefaultCurrency sets DefaultCurrency field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


