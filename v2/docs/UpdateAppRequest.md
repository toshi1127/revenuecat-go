# UpdateAppRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** | The name of the app | [optional] 
**Amazon** | Pointer to [**UpdateAppRequestAmazon**](UpdateAppRequestAmazon.md) |  | [optional] 
**AppStore** | Pointer to [**UpdateAppRequestAppStore**](UpdateAppRequestAppStore.md) |  | [optional] 
**MacAppStore** | Pointer to [**UpdateAppRequestMacAppStore**](UpdateAppRequestMacAppStore.md) |  | [optional] 
**PlayStore** | Pointer to [**UpdateAppRequestPlayStore**](UpdateAppRequestPlayStore.md) |  | [optional] 
**Stripe** | Pointer to [**UpdateAppRequestStripe**](UpdateAppRequestStripe.md) |  | [optional] 
**RcBilling** | Pointer to [**UpdateAppRequestRcBilling**](UpdateAppRequestRcBilling.md) |  | [optional] 
**Roku** | Pointer to [**UpdateAppRequestRoku**](UpdateAppRequestRoku.md) |  | [optional] 
**Paddle** | Pointer to [**UpdateAppRequestPaddle**](UpdateAppRequestPaddle.md) |  | [optional] 

## Methods

### NewUpdateAppRequest

`func NewUpdateAppRequest() *UpdateAppRequest`

NewUpdateAppRequest instantiates a new UpdateAppRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAppRequestWithDefaults

`func NewUpdateAppRequestWithDefaults() *UpdateAppRequest`

NewUpdateAppRequestWithDefaults instantiates a new UpdateAppRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateAppRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateAppRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateAppRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateAppRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetAmazon

`func (o *UpdateAppRequest) GetAmazon() UpdateAppRequestAmazon`

GetAmazon returns the Amazon field if non-nil, zero value otherwise.

### GetAmazonOk

`func (o *UpdateAppRequest) GetAmazonOk() (*UpdateAppRequestAmazon, bool)`

GetAmazonOk returns a tuple with the Amazon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmazon

`func (o *UpdateAppRequest) SetAmazon(v UpdateAppRequestAmazon)`

SetAmazon sets Amazon field to given value.

### HasAmazon

`func (o *UpdateAppRequest) HasAmazon() bool`

HasAmazon returns a boolean if a field has been set.

### GetAppStore

`func (o *UpdateAppRequest) GetAppStore() UpdateAppRequestAppStore`

GetAppStore returns the AppStore field if non-nil, zero value otherwise.

### GetAppStoreOk

`func (o *UpdateAppRequest) GetAppStoreOk() (*UpdateAppRequestAppStore, bool)`

GetAppStoreOk returns a tuple with the AppStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppStore

`func (o *UpdateAppRequest) SetAppStore(v UpdateAppRequestAppStore)`

SetAppStore sets AppStore field to given value.

### HasAppStore

`func (o *UpdateAppRequest) HasAppStore() bool`

HasAppStore returns a boolean if a field has been set.

### GetMacAppStore

`func (o *UpdateAppRequest) GetMacAppStore() UpdateAppRequestMacAppStore`

GetMacAppStore returns the MacAppStore field if non-nil, zero value otherwise.

### GetMacAppStoreOk

`func (o *UpdateAppRequest) GetMacAppStoreOk() (*UpdateAppRequestMacAppStore, bool)`

GetMacAppStoreOk returns a tuple with the MacAppStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMacAppStore

`func (o *UpdateAppRequest) SetMacAppStore(v UpdateAppRequestMacAppStore)`

SetMacAppStore sets MacAppStore field to given value.

### HasMacAppStore

`func (o *UpdateAppRequest) HasMacAppStore() bool`

HasMacAppStore returns a boolean if a field has been set.

### GetPlayStore

`func (o *UpdateAppRequest) GetPlayStore() UpdateAppRequestPlayStore`

GetPlayStore returns the PlayStore field if non-nil, zero value otherwise.

### GetPlayStoreOk

`func (o *UpdateAppRequest) GetPlayStoreOk() (*UpdateAppRequestPlayStore, bool)`

GetPlayStoreOk returns a tuple with the PlayStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlayStore

`func (o *UpdateAppRequest) SetPlayStore(v UpdateAppRequestPlayStore)`

SetPlayStore sets PlayStore field to given value.

### HasPlayStore

`func (o *UpdateAppRequest) HasPlayStore() bool`

HasPlayStore returns a boolean if a field has been set.

### GetStripe

`func (o *UpdateAppRequest) GetStripe() UpdateAppRequestStripe`

GetStripe returns the Stripe field if non-nil, zero value otherwise.

### GetStripeOk

`func (o *UpdateAppRequest) GetStripeOk() (*UpdateAppRequestStripe, bool)`

GetStripeOk returns a tuple with the Stripe field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripe

`func (o *UpdateAppRequest) SetStripe(v UpdateAppRequestStripe)`

SetStripe sets Stripe field to given value.

### HasStripe

`func (o *UpdateAppRequest) HasStripe() bool`

HasStripe returns a boolean if a field has been set.

### GetRcBilling

`func (o *UpdateAppRequest) GetRcBilling() UpdateAppRequestRcBilling`

GetRcBilling returns the RcBilling field if non-nil, zero value otherwise.

### GetRcBillingOk

`func (o *UpdateAppRequest) GetRcBillingOk() (*UpdateAppRequestRcBilling, bool)`

GetRcBillingOk returns a tuple with the RcBilling field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRcBilling

`func (o *UpdateAppRequest) SetRcBilling(v UpdateAppRequestRcBilling)`

SetRcBilling sets RcBilling field to given value.

### HasRcBilling

`func (o *UpdateAppRequest) HasRcBilling() bool`

HasRcBilling returns a boolean if a field has been set.

### GetRoku

`func (o *UpdateAppRequest) GetRoku() UpdateAppRequestRoku`

GetRoku returns the Roku field if non-nil, zero value otherwise.

### GetRokuOk

`func (o *UpdateAppRequest) GetRokuOk() (*UpdateAppRequestRoku, bool)`

GetRokuOk returns a tuple with the Roku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoku

`func (o *UpdateAppRequest) SetRoku(v UpdateAppRequestRoku)`

SetRoku sets Roku field to given value.

### HasRoku

`func (o *UpdateAppRequest) HasRoku() bool`

HasRoku returns a boolean if a field has been set.

### GetPaddle

`func (o *UpdateAppRequest) GetPaddle() UpdateAppRequestPaddle`

GetPaddle returns the Paddle field if non-nil, zero value otherwise.

### GetPaddleOk

`func (o *UpdateAppRequest) GetPaddleOk() (*UpdateAppRequestPaddle, bool)`

GetPaddleOk returns a tuple with the Paddle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaddle

`func (o *UpdateAppRequest) SetPaddle(v UpdateAppRequestPaddle)`

SetPaddle sets Paddle field to given value.

### HasPaddle

`func (o *UpdateAppRequest) HasPaddle() bool`

HasPaddle returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


