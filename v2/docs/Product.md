# Product

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. Always has the value &#x60;list&#x60;. | 
**Id** | **string** | The id of the product | 
**StoreIdentifier** | **string** | The store product identifier | 
**Type** | [**ProductType**](ProductType.md) |  | 
**Subscription** | Pointer to [**NullableSubscriptionProduct**](SubscriptionProduct.md) |  | [optional] 
**OneTime** | Pointer to [**NullableOneTimeProduct**](OneTimeProduct.md) |  | [optional] 
**CreatedAt** | **int64** | The date when the product was created in ms since epoch | 
**AppId** | **string** | The id of the app | 
**App** | Pointer to [**App**](App.md) |  | [optional] 
**DisplayName** | **NullableString** | The display name of the product | 

## Methods

### NewProduct

`func NewProduct(object string, id string, storeIdentifier string, type_ ProductType, createdAt int64, appId string, displayName NullableString, ) *Product`

NewProduct instantiates a new Product object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductWithDefaults

`func NewProductWithDefaults() *Product`

NewProductWithDefaults instantiates a new Product object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Product) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Product) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Product) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *Product) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Product) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Product) SetId(v string)`

SetId sets Id field to given value.


### GetStoreIdentifier

`func (o *Product) GetStoreIdentifier() string`

GetStoreIdentifier returns the StoreIdentifier field if non-nil, zero value otherwise.

### GetStoreIdentifierOk

`func (o *Product) GetStoreIdentifierOk() (*string, bool)`

GetStoreIdentifierOk returns a tuple with the StoreIdentifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStoreIdentifier

`func (o *Product) SetStoreIdentifier(v string)`

SetStoreIdentifier sets StoreIdentifier field to given value.


### GetType

`func (o *Product) GetType() ProductType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Product) GetTypeOk() (*ProductType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Product) SetType(v ProductType)`

SetType sets Type field to given value.


### GetSubscription

`func (o *Product) GetSubscription() SubscriptionProduct`

GetSubscription returns the Subscription field if non-nil, zero value otherwise.

### GetSubscriptionOk

`func (o *Product) GetSubscriptionOk() (*SubscriptionProduct, bool)`

GetSubscriptionOk returns a tuple with the Subscription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscription

`func (o *Product) SetSubscription(v SubscriptionProduct)`

SetSubscription sets Subscription field to given value.

### HasSubscription

`func (o *Product) HasSubscription() bool`

HasSubscription returns a boolean if a field has been set.

### SetSubscriptionNil

`func (o *Product) SetSubscriptionNil(b bool)`

 SetSubscriptionNil sets the value for Subscription to be an explicit nil

### UnsetSubscription
`func (o *Product) UnsetSubscription()`

UnsetSubscription ensures that no value is present for Subscription, not even an explicit nil
### GetOneTime

`func (o *Product) GetOneTime() OneTimeProduct`

GetOneTime returns the OneTime field if non-nil, zero value otherwise.

### GetOneTimeOk

`func (o *Product) GetOneTimeOk() (*OneTimeProduct, bool)`

GetOneTimeOk returns a tuple with the OneTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOneTime

`func (o *Product) SetOneTime(v OneTimeProduct)`

SetOneTime sets OneTime field to given value.

### HasOneTime

`func (o *Product) HasOneTime() bool`

HasOneTime returns a boolean if a field has been set.

### SetOneTimeNil

`func (o *Product) SetOneTimeNil(b bool)`

 SetOneTimeNil sets the value for OneTime to be an explicit nil

### UnsetOneTime
`func (o *Product) UnsetOneTime()`

UnsetOneTime ensures that no value is present for OneTime, not even an explicit nil
### GetCreatedAt

`func (o *Product) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Product) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Product) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.


### GetAppId

`func (o *Product) GetAppId() string`

GetAppId returns the AppId field if non-nil, zero value otherwise.

### GetAppIdOk

`func (o *Product) GetAppIdOk() (*string, bool)`

GetAppIdOk returns a tuple with the AppId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppId

`func (o *Product) SetAppId(v string)`

SetAppId sets AppId field to given value.


### GetApp

`func (o *Product) GetApp() App`

GetApp returns the App field if non-nil, zero value otherwise.

### GetAppOk

`func (o *Product) GetAppOk() (*App, bool)`

GetAppOk returns a tuple with the App field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApp

`func (o *Product) SetApp(v App)`

SetApp sets App field to given value.

### HasApp

`func (o *Product) HasApp() bool`

HasApp returns a boolean if a field has been set.

### GetDisplayName

`func (o *Product) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *Product) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *Product) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.


### SetDisplayNameNil

`func (o *Product) SetDisplayNameNil(b bool)`

 SetDisplayNameNil sets the value for DisplayName to be an explicit nil

### UnsetDisplayName
`func (o *Product) UnsetDisplayName()`

UnsetDisplayName ensures that no value is present for DisplayName, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


