# AppCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Amazon** | Pointer to [**AmazonAppCreateAmazon**](AmazonAppCreateAmazon.md) |  | [optional] 
**AppStore** | Pointer to [**AppStoreAppCreateAppStore**](AppStoreAppCreateAppStore.md) |  | [optional] 
**MacAppStore** | Pointer to [**MacAppStoreAppCreateMacAppStore**](MacAppStoreAppCreateMacAppStore.md) |  | [optional] 
**PlayStore** | Pointer to [**UpdateAppRequestPlayStore**](UpdateAppRequestPlayStore.md) |  | [optional] 
**Stripe** | Pointer to [**StripeAppCreateStripe**](StripeAppCreateStripe.md) |  | [optional] 
**RcBilling** | Pointer to [**NullableRCBillingAppCreateRcBilling**](RCBillingAppCreateRcBilling.md) |  | [optional] 
**Roku** | Pointer to [**NullableRokuAppCreateRoku**](RokuAppCreateRoku.md) |  | [optional] 
**Paddle** | Pointer to [**NullablePaddleAppCreatePaddle**](PaddleAppCreatePaddle.md) |  | [optional] 
**Name** | **string** | The name of the app | 
**Type** | **string** | The platform of the app. Mac App Store is disabled by default. See [Legacy Mac Apps](https://www.revenuecat.com/docs/legacy-mac-apps) for more details.  | 

## Methods

### NewAppCreate

`func NewAppCreate(name string, type_ string, ) *AppCreate`

NewAppCreate instantiates a new AppCreate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAppCreateWithDefaults

`func NewAppCreateWithDefaults() *AppCreate`

NewAppCreateWithDefaults instantiates a new AppCreate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAmazon

`func (o *AppCreate) GetAmazon() AmazonAppCreateAmazon`

GetAmazon returns the Amazon field if non-nil, zero value otherwise.

### GetAmazonOk

`func (o *AppCreate) GetAmazonOk() (*AmazonAppCreateAmazon, bool)`

GetAmazonOk returns a tuple with the Amazon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmazon

`func (o *AppCreate) SetAmazon(v AmazonAppCreateAmazon)`

SetAmazon sets Amazon field to given value.

### HasAmazon

`func (o *AppCreate) HasAmazon() bool`

HasAmazon returns a boolean if a field has been set.

### GetAppStore

`func (o *AppCreate) GetAppStore() AppStoreAppCreateAppStore`

GetAppStore returns the AppStore field if non-nil, zero value otherwise.

### GetAppStoreOk

`func (o *AppCreate) GetAppStoreOk() (*AppStoreAppCreateAppStore, bool)`

GetAppStoreOk returns a tuple with the AppStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppStore

`func (o *AppCreate) SetAppStore(v AppStoreAppCreateAppStore)`

SetAppStore sets AppStore field to given value.

### HasAppStore

`func (o *AppCreate) HasAppStore() bool`

HasAppStore returns a boolean if a field has been set.

### GetMacAppStore

`func (o *AppCreate) GetMacAppStore() MacAppStoreAppCreateMacAppStore`

GetMacAppStore returns the MacAppStore field if non-nil, zero value otherwise.

### GetMacAppStoreOk

`func (o *AppCreate) GetMacAppStoreOk() (*MacAppStoreAppCreateMacAppStore, bool)`

GetMacAppStoreOk returns a tuple with the MacAppStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMacAppStore

`func (o *AppCreate) SetMacAppStore(v MacAppStoreAppCreateMacAppStore)`

SetMacAppStore sets MacAppStore field to given value.

### HasMacAppStore

`func (o *AppCreate) HasMacAppStore() bool`

HasMacAppStore returns a boolean if a field has been set.

### GetPlayStore

`func (o *AppCreate) GetPlayStore() UpdateAppRequestPlayStore`

GetPlayStore returns the PlayStore field if non-nil, zero value otherwise.

### GetPlayStoreOk

`func (o *AppCreate) GetPlayStoreOk() (*UpdateAppRequestPlayStore, bool)`

GetPlayStoreOk returns a tuple with the PlayStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlayStore

`func (o *AppCreate) SetPlayStore(v UpdateAppRequestPlayStore)`

SetPlayStore sets PlayStore field to given value.

### HasPlayStore

`func (o *AppCreate) HasPlayStore() bool`

HasPlayStore returns a boolean if a field has been set.

### GetStripe

`func (o *AppCreate) GetStripe() StripeAppCreateStripe`

GetStripe returns the Stripe field if non-nil, zero value otherwise.

### GetStripeOk

`func (o *AppCreate) GetStripeOk() (*StripeAppCreateStripe, bool)`

GetStripeOk returns a tuple with the Stripe field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripe

`func (o *AppCreate) SetStripe(v StripeAppCreateStripe)`

SetStripe sets Stripe field to given value.

### HasStripe

`func (o *AppCreate) HasStripe() bool`

HasStripe returns a boolean if a field has been set.

### GetRcBilling

`func (o *AppCreate) GetRcBilling() RCBillingAppCreateRcBilling`

GetRcBilling returns the RcBilling field if non-nil, zero value otherwise.

### GetRcBillingOk

`func (o *AppCreate) GetRcBillingOk() (*RCBillingAppCreateRcBilling, bool)`

GetRcBillingOk returns a tuple with the RcBilling field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRcBilling

`func (o *AppCreate) SetRcBilling(v RCBillingAppCreateRcBilling)`

SetRcBilling sets RcBilling field to given value.

### HasRcBilling

`func (o *AppCreate) HasRcBilling() bool`

HasRcBilling returns a boolean if a field has been set.

### SetRcBillingNil

`func (o *AppCreate) SetRcBillingNil(b bool)`

 SetRcBillingNil sets the value for RcBilling to be an explicit nil

### UnsetRcBilling
`func (o *AppCreate) UnsetRcBilling()`

UnsetRcBilling ensures that no value is present for RcBilling, not even an explicit nil
### GetRoku

`func (o *AppCreate) GetRoku() RokuAppCreateRoku`

GetRoku returns the Roku field if non-nil, zero value otherwise.

### GetRokuOk

`func (o *AppCreate) GetRokuOk() (*RokuAppCreateRoku, bool)`

GetRokuOk returns a tuple with the Roku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoku

`func (o *AppCreate) SetRoku(v RokuAppCreateRoku)`

SetRoku sets Roku field to given value.

### HasRoku

`func (o *AppCreate) HasRoku() bool`

HasRoku returns a boolean if a field has been set.

### SetRokuNil

`func (o *AppCreate) SetRokuNil(b bool)`

 SetRokuNil sets the value for Roku to be an explicit nil

### UnsetRoku
`func (o *AppCreate) UnsetRoku()`

UnsetRoku ensures that no value is present for Roku, not even an explicit nil
### GetPaddle

`func (o *AppCreate) GetPaddle() PaddleAppCreatePaddle`

GetPaddle returns the Paddle field if non-nil, zero value otherwise.

### GetPaddleOk

`func (o *AppCreate) GetPaddleOk() (*PaddleAppCreatePaddle, bool)`

GetPaddleOk returns a tuple with the Paddle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaddle

`func (o *AppCreate) SetPaddle(v PaddleAppCreatePaddle)`

SetPaddle sets Paddle field to given value.

### HasPaddle

`func (o *AppCreate) HasPaddle() bool`

HasPaddle returns a boolean if a field has been set.

### SetPaddleNil

`func (o *AppCreate) SetPaddleNil(b bool)`

 SetPaddleNil sets the value for Paddle to be an explicit nil

### UnsetPaddle
`func (o *AppCreate) UnsetPaddle()`

UnsetPaddle ensures that no value is present for Paddle, not even an explicit nil
### GetName

`func (o *AppCreate) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AppCreate) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AppCreate) SetName(v string)`

SetName sets Name field to given value.


### GetType

`func (o *AppCreate) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *AppCreate) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *AppCreate) SetType(v string)`

SetType sets Type field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


