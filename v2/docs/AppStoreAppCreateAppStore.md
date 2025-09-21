# AppStoreAppCreateAppStore

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BundleId** | **string** | The bundle ID of the app | 
**SharedSecret** | Pointer to **string** | The shared secret of the app | [optional] 
**SubscriptionPrivateKey** | Pointer to **string** | PKCS /#8 In App Key downloaded from App Store Connect in PEM format. Copy the contents of the file in this field. See instructions on how to get it in:  https://www.revenuecat.com/docs/in-app-purchase-key-configuration  | [optional] 
**SubscriptionKeyId** | Pointer to **string** | In App Key id. The ID of the downloaded in app key. You can get it from App Store Connect | [optional] 
**SubscriptionKeyIssuer** | Pointer to **string** | The key Issuer id. See instructions on how to obtain this in: https://www.revenuecat.com/docs/in-app-purchase-key-configuration#3-providing-the-issuer-id-to-revenuecat  | [optional] 

## Methods

### NewAppStoreAppCreateAppStore

`func NewAppStoreAppCreateAppStore(bundleId string, ) *AppStoreAppCreateAppStore`

NewAppStoreAppCreateAppStore instantiates a new AppStoreAppCreateAppStore object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAppStoreAppCreateAppStoreWithDefaults

`func NewAppStoreAppCreateAppStoreWithDefaults() *AppStoreAppCreateAppStore`

NewAppStoreAppCreateAppStoreWithDefaults instantiates a new AppStoreAppCreateAppStore object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBundleId

`func (o *AppStoreAppCreateAppStore) GetBundleId() string`

GetBundleId returns the BundleId field if non-nil, zero value otherwise.

### GetBundleIdOk

`func (o *AppStoreAppCreateAppStore) GetBundleIdOk() (*string, bool)`

GetBundleIdOk returns a tuple with the BundleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBundleId

`func (o *AppStoreAppCreateAppStore) SetBundleId(v string)`

SetBundleId sets BundleId field to given value.


### GetSharedSecret

`func (o *AppStoreAppCreateAppStore) GetSharedSecret() string`

GetSharedSecret returns the SharedSecret field if non-nil, zero value otherwise.

### GetSharedSecretOk

`func (o *AppStoreAppCreateAppStore) GetSharedSecretOk() (*string, bool)`

GetSharedSecretOk returns a tuple with the SharedSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSharedSecret

`func (o *AppStoreAppCreateAppStore) SetSharedSecret(v string)`

SetSharedSecret sets SharedSecret field to given value.

### HasSharedSecret

`func (o *AppStoreAppCreateAppStore) HasSharedSecret() bool`

HasSharedSecret returns a boolean if a field has been set.

### GetSubscriptionPrivateKey

`func (o *AppStoreAppCreateAppStore) GetSubscriptionPrivateKey() string`

GetSubscriptionPrivateKey returns the SubscriptionPrivateKey field if non-nil, zero value otherwise.

### GetSubscriptionPrivateKeyOk

`func (o *AppStoreAppCreateAppStore) GetSubscriptionPrivateKeyOk() (*string, bool)`

GetSubscriptionPrivateKeyOk returns a tuple with the SubscriptionPrivateKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionPrivateKey

`func (o *AppStoreAppCreateAppStore) SetSubscriptionPrivateKey(v string)`

SetSubscriptionPrivateKey sets SubscriptionPrivateKey field to given value.

### HasSubscriptionPrivateKey

`func (o *AppStoreAppCreateAppStore) HasSubscriptionPrivateKey() bool`

HasSubscriptionPrivateKey returns a boolean if a field has been set.

### GetSubscriptionKeyId

`func (o *AppStoreAppCreateAppStore) GetSubscriptionKeyId() string`

GetSubscriptionKeyId returns the SubscriptionKeyId field if non-nil, zero value otherwise.

### GetSubscriptionKeyIdOk

`func (o *AppStoreAppCreateAppStore) GetSubscriptionKeyIdOk() (*string, bool)`

GetSubscriptionKeyIdOk returns a tuple with the SubscriptionKeyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionKeyId

`func (o *AppStoreAppCreateAppStore) SetSubscriptionKeyId(v string)`

SetSubscriptionKeyId sets SubscriptionKeyId field to given value.

### HasSubscriptionKeyId

`func (o *AppStoreAppCreateAppStore) HasSubscriptionKeyId() bool`

HasSubscriptionKeyId returns a boolean if a field has been set.

### GetSubscriptionKeyIssuer

`func (o *AppStoreAppCreateAppStore) GetSubscriptionKeyIssuer() string`

GetSubscriptionKeyIssuer returns the SubscriptionKeyIssuer field if non-nil, zero value otherwise.

### GetSubscriptionKeyIssuerOk

`func (o *AppStoreAppCreateAppStore) GetSubscriptionKeyIssuerOk() (*string, bool)`

GetSubscriptionKeyIssuerOk returns a tuple with the SubscriptionKeyIssuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptionKeyIssuer

`func (o *AppStoreAppCreateAppStore) SetSubscriptionKeyIssuer(v string)`

SetSubscriptionKeyIssuer sets SubscriptionKeyIssuer field to given value.

### HasSubscriptionKeyIssuer

`func (o *AppStoreAppCreateAppStore) HasSubscriptionKeyIssuer() bool`

HasSubscriptionKeyIssuer returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


