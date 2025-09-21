# AppAllOf

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The id of the app | 
**Name** | **string** | The name of the app | 
**CreatedAt** | **int64** | The date when the app was created in ms since epoch | 
**Type** | **string** | The platform of the app | 
**ProjectId** | **string** | The id of the project | 

## Methods

### NewAppAllOf

`func NewAppAllOf(object string, id string, name string, createdAt int64, type_ string, projectId string, ) *AppAllOf`

NewAppAllOf instantiates a new AppAllOf object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAppAllOfWithDefaults

`func NewAppAllOfWithDefaults() *AppAllOf`

NewAppAllOfWithDefaults instantiates a new AppAllOf object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *AppAllOf) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *AppAllOf) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *AppAllOf) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *AppAllOf) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AppAllOf) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AppAllOf) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *AppAllOf) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AppAllOf) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AppAllOf) SetName(v string)`

SetName sets Name field to given value.


### GetCreatedAt

`func (o *AppAllOf) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *AppAllOf) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *AppAllOf) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.


### GetType

`func (o *AppAllOf) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *AppAllOf) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *AppAllOf) SetType(v string)`

SetType sets Type field to given value.


### GetProjectId

`func (o *AppAllOf) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *AppAllOf) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *AppAllOf) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


