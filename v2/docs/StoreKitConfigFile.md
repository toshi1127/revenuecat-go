# StoreKitConfigFile

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Contents** | **map[string]interface{}** | Contents of the StoreKit config file | 

## Methods

### NewStoreKitConfigFile

`func NewStoreKitConfigFile(object string, contents map[string]interface{}, ) *StoreKitConfigFile`

NewStoreKitConfigFile instantiates a new StoreKitConfigFile object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStoreKitConfigFileWithDefaults

`func NewStoreKitConfigFileWithDefaults() *StoreKitConfigFile`

NewStoreKitConfigFileWithDefaults instantiates a new StoreKitConfigFile object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *StoreKitConfigFile) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *StoreKitConfigFile) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *StoreKitConfigFile) SetObject(v string)`

SetObject sets Object field to given value.


### GetContents

`func (o *StoreKitConfigFile) GetContents() map[string]interface{}`

GetContents returns the Contents field if non-nil, zero value otherwise.

### GetContentsOk

`func (o *StoreKitConfigFile) GetContentsOk() (*map[string]interface{}, bool)`

GetContentsOk returns a tuple with the Contents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContents

`func (o *StoreKitConfigFile) SetContents(v map[string]interface{})`

SetContents sets Contents field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


