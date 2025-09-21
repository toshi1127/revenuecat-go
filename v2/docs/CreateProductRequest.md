# CreateProductRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StoreIdentifier** | **string** | The store identifier of the product. - For Apple App Store products this is the product ID of the subscription or in-app product. - For Google&#39;s Play Store, it should follow the format &#39;productId:basePlanId&#39; for subscription products and SKU for one-time purchase products. - For Stripe, the product identifier that always starts with \&quot;prod_\&quot; - For Amazon, if it&#39;s a subscription, the term SKU of the subscription. If it&#39;s a one-time purchase, the SKU of the product. - For Roku, this is the product identifier of the subscription or one-time purchase product.  | 
**AppId** | **string** | The ID of the app | 
**Type** | [**ProductType**](ProductType.md) |  | 
**DisplayName** | Pointer to **NullableString** | The display name of the product | [optional] 

## Methods

### NewCreateProductRequest

`func NewCreateProductRequest(storeIdentifier string, appId string, type_ ProductType, ) *CreateProductRequest`

NewCreateProductRequest instantiates a new CreateProductRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateProductRequestWithDefaults

`func NewCreateProductRequestWithDefaults() *CreateProductRequest`

NewCreateProductRequestWithDefaults instantiates a new CreateProductRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStoreIdentifier

`func (o *CreateProductRequest) GetStoreIdentifier() string`

GetStoreIdentifier returns the StoreIdentifier field if non-nil, zero value otherwise.

### GetStoreIdentifierOk

`func (o *CreateProductRequest) GetStoreIdentifierOk() (*string, bool)`

GetStoreIdentifierOk returns a tuple with the StoreIdentifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStoreIdentifier

`func (o *CreateProductRequest) SetStoreIdentifier(v string)`

SetStoreIdentifier sets StoreIdentifier field to given value.


### GetAppId

`func (o *CreateProductRequest) GetAppId() string`

GetAppId returns the AppId field if non-nil, zero value otherwise.

### GetAppIdOk

`func (o *CreateProductRequest) GetAppIdOk() (*string, bool)`

GetAppIdOk returns a tuple with the AppId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppId

`func (o *CreateProductRequest) SetAppId(v string)`

SetAppId sets AppId field to given value.


### GetType

`func (o *CreateProductRequest) GetType() ProductType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateProductRequest) GetTypeOk() (*ProductType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateProductRequest) SetType(v ProductType)`

SetType sets Type field to given value.


### GetDisplayName

`func (o *CreateProductRequest) GetDisplayName() string`

GetDisplayName returns the DisplayName field if non-nil, zero value otherwise.

### GetDisplayNameOk

`func (o *CreateProductRequest) GetDisplayNameOk() (*string, bool)`

GetDisplayNameOk returns a tuple with the DisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayName

`func (o *CreateProductRequest) SetDisplayName(v string)`

SetDisplayName sets DisplayName field to given value.

### HasDisplayName

`func (o *CreateProductRequest) HasDisplayName() bool`

HasDisplayName returns a boolean if a field has been set.

### SetDisplayNameNil

`func (o *CreateProductRequest) SetDisplayNameNil(b bool)`

 SetDisplayNameNil sets the value for DisplayName to be an explicit nil

### UnsetDisplayName
`func (o *CreateProductRequest) UnsetDisplayName()`

UnsetDisplayName ensures that no value is present for DisplayName, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


