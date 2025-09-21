# DeletedObject

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | The type of the deleted object | 
**Id** | **string** | The ID of the deleted object | 
**DeletedAt** | **int64** | The date when the object was deleted in ms since epoch | 

## Methods

### NewDeletedObject

`func NewDeletedObject(object string, id string, deletedAt int64, ) *DeletedObject`

NewDeletedObject instantiates a new DeletedObject object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeletedObjectWithDefaults

`func NewDeletedObjectWithDefaults() *DeletedObject`

NewDeletedObjectWithDefaults instantiates a new DeletedObject object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *DeletedObject) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *DeletedObject) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *DeletedObject) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *DeletedObject) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DeletedObject) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DeletedObject) SetId(v string)`

SetId sets Id field to given value.


### GetDeletedAt

`func (o *DeletedObject) GetDeletedAt() int64`

GetDeletedAt returns the DeletedAt field if non-nil, zero value otherwise.

### GetDeletedAtOk

`func (o *DeletedObject) GetDeletedAtOk() (*int64, bool)`

GetDeletedAtOk returns a tuple with the DeletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeletedAt

`func (o *DeletedObject) SetDeletedAt(v int64)`

SetDeletedAt sets DeletedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


