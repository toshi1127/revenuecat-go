# App

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Amazon** | Pointer to [**AmazonAppAmazon**](AmazonAppAmazon.md) |  | [optional] 
**AppStore** | Pointer to [**AppStoreAppAppStore**](AppStoreAppAppStore.md) |  | [optional] 
**MacAppStore** | Pointer to [**MacAppStoreAppMacAppStore**](MacAppStoreAppMacAppStore.md) |  | [optional] 
**PlayStore** | Pointer to [**PlayStoreAppPlayStore**](PlayStoreAppPlayStore.md) |  | [optional] 
**Stripe** | Pointer to [**StripeAppStripe**](StripeAppStripe.md) |  | [optional] 
**RcBilling** | Pointer to [**RCBillingAppRcBilling**](RCBillingAppRcBilling.md) |  | [optional] 
**Roku** | Pointer to [**RokuAppRoku**](RokuAppRoku.md) |  | [optional] 
**Paddle** | Pointer to [**PaddleAppPaddle**](PaddleAppPaddle.md) |  | [optional] 
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The id of the app | 
**Name** | **string** | The name of the app | 
**CreatedAt** | **int64** | The date when the app was created in ms since epoch | 
**Type** | **string** | The platform of the app | 
**ProjectId** | **string** | The id of the project | 

## Methods

### NewApp

`func NewApp(object string, id string, name string, createdAt int64, type_ string, projectId string, ) *App`

NewApp instantiates a new App object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAppWithDefaults

`func NewAppWithDefaults() *App`

NewAppWithDefaults instantiates a new App object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAmazon

`func (o *App) GetAmazon() AmazonAppAmazon`

GetAmazon returns the Amazon field if non-nil, zero value otherwise.

### GetAmazonOk

`func (o *App) GetAmazonOk() (*AmazonAppAmazon, bool)`

GetAmazonOk returns a tuple with the Amazon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAmazon

`func (o *App) SetAmazon(v AmazonAppAmazon)`

SetAmazon sets Amazon field to given value.

### HasAmazon

`func (o *App) HasAmazon() bool`

HasAmazon returns a boolean if a field has been set.

### GetAppStore

`func (o *App) GetAppStore() AppStoreAppAppStore`

GetAppStore returns the AppStore field if non-nil, zero value otherwise.

### GetAppStoreOk

`func (o *App) GetAppStoreOk() (*AppStoreAppAppStore, bool)`

GetAppStoreOk returns a tuple with the AppStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppStore

`func (o *App) SetAppStore(v AppStoreAppAppStore)`

SetAppStore sets AppStore field to given value.

### HasAppStore

`func (o *App) HasAppStore() bool`

HasAppStore returns a boolean if a field has been set.

### GetMacAppStore

`func (o *App) GetMacAppStore() MacAppStoreAppMacAppStore`

GetMacAppStore returns the MacAppStore field if non-nil, zero value otherwise.

### GetMacAppStoreOk

`func (o *App) GetMacAppStoreOk() (*MacAppStoreAppMacAppStore, bool)`

GetMacAppStoreOk returns a tuple with the MacAppStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMacAppStore

`func (o *App) SetMacAppStore(v MacAppStoreAppMacAppStore)`

SetMacAppStore sets MacAppStore field to given value.

### HasMacAppStore

`func (o *App) HasMacAppStore() bool`

HasMacAppStore returns a boolean if a field has been set.

### GetPlayStore

`func (o *App) GetPlayStore() PlayStoreAppPlayStore`

GetPlayStore returns the PlayStore field if non-nil, zero value otherwise.

### GetPlayStoreOk

`func (o *App) GetPlayStoreOk() (*PlayStoreAppPlayStore, bool)`

GetPlayStoreOk returns a tuple with the PlayStore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlayStore

`func (o *App) SetPlayStore(v PlayStoreAppPlayStore)`

SetPlayStore sets PlayStore field to given value.

### HasPlayStore

`func (o *App) HasPlayStore() bool`

HasPlayStore returns a boolean if a field has been set.

### GetStripe

`func (o *App) GetStripe() StripeAppStripe`

GetStripe returns the Stripe field if non-nil, zero value otherwise.

### GetStripeOk

`func (o *App) GetStripeOk() (*StripeAppStripe, bool)`

GetStripeOk returns a tuple with the Stripe field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripe

`func (o *App) SetStripe(v StripeAppStripe)`

SetStripe sets Stripe field to given value.

### HasStripe

`func (o *App) HasStripe() bool`

HasStripe returns a boolean if a field has been set.

### GetRcBilling

`func (o *App) GetRcBilling() RCBillingAppRcBilling`

GetRcBilling returns the RcBilling field if non-nil, zero value otherwise.

### GetRcBillingOk

`func (o *App) GetRcBillingOk() (*RCBillingAppRcBilling, bool)`

GetRcBillingOk returns a tuple with the RcBilling field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRcBilling

`func (o *App) SetRcBilling(v RCBillingAppRcBilling)`

SetRcBilling sets RcBilling field to given value.

### HasRcBilling

`func (o *App) HasRcBilling() bool`

HasRcBilling returns a boolean if a field has been set.

### GetRoku

`func (o *App) GetRoku() RokuAppRoku`

GetRoku returns the Roku field if non-nil, zero value otherwise.

### GetRokuOk

`func (o *App) GetRokuOk() (*RokuAppRoku, bool)`

GetRokuOk returns a tuple with the Roku field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoku

`func (o *App) SetRoku(v RokuAppRoku)`

SetRoku sets Roku field to given value.

### HasRoku

`func (o *App) HasRoku() bool`

HasRoku returns a boolean if a field has been set.

### GetPaddle

`func (o *App) GetPaddle() PaddleAppPaddle`

GetPaddle returns the Paddle field if non-nil, zero value otherwise.

### GetPaddleOk

`func (o *App) GetPaddleOk() (*PaddleAppPaddle, bool)`

GetPaddleOk returns a tuple with the Paddle field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaddle

`func (o *App) SetPaddle(v PaddleAppPaddle)`

SetPaddle sets Paddle field to given value.

### HasPaddle

`func (o *App) HasPaddle() bool`

HasPaddle returns a boolean if a field has been set.

### GetObject

`func (o *App) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *App) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *App) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *App) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *App) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *App) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *App) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *App) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *App) SetName(v string)`

SetName sets Name field to given value.


### GetCreatedAt

`func (o *App) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *App) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *App) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.


### GetType

`func (o *App) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *App) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *App) SetType(v string)`

SetType sets Type field to given value.


### GetProjectId

`func (o *App) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *App) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *App) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


