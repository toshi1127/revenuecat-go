# Paywall

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | The id of the paywall | 
**Name** | **NullableString** | The name of the paywall | 
**OfferingId** | **string** | The ID of the offering the paywall is for. | 
**CreatedAt** | **int64** | The date the paywall was created at in ms since epoch | 
**PublishedAt** | **NullableInt64** | The date the paywall was published at in ms since epoch | 

## Methods

### NewPaywall

`func NewPaywall(object string, id string, name NullableString, offeringId string, createdAt int64, publishedAt NullableInt64, ) *Paywall`

NewPaywall instantiates a new Paywall object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaywallWithDefaults

`func NewPaywallWithDefaults() *Paywall`

NewPaywallWithDefaults instantiates a new Paywall object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Paywall) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Paywall) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Paywall) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *Paywall) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Paywall) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Paywall) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *Paywall) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Paywall) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Paywall) SetName(v string)`

SetName sets Name field to given value.


### SetNameNil

`func (o *Paywall) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *Paywall) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetOfferingId

`func (o *Paywall) GetOfferingId() string`

GetOfferingId returns the OfferingId field if non-nil, zero value otherwise.

### GetOfferingIdOk

`func (o *Paywall) GetOfferingIdOk() (*string, bool)`

GetOfferingIdOk returns a tuple with the OfferingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOfferingId

`func (o *Paywall) SetOfferingId(v string)`

SetOfferingId sets OfferingId field to given value.


### GetCreatedAt

`func (o *Paywall) GetCreatedAt() int64`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Paywall) GetCreatedAtOk() (*int64, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Paywall) SetCreatedAt(v int64)`

SetCreatedAt sets CreatedAt field to given value.


### GetPublishedAt

`func (o *Paywall) GetPublishedAt() int64`

GetPublishedAt returns the PublishedAt field if non-nil, zero value otherwise.

### GetPublishedAtOk

`func (o *Paywall) GetPublishedAtOk() (*int64, bool)`

GetPublishedAtOk returns a tuple with the PublishedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublishedAt

`func (o *Paywall) SetPublishedAt(v int64)`

SetPublishedAt sets PublishedAt field to given value.


### SetPublishedAtNil

`func (o *Paywall) SetPublishedAtNil(b bool)`

 SetPublishedAtNil sets the value for PublishedAt to be an explicit nil

### UnsetPublishedAt
`func (o *Paywall) UnsetPublishedAt()`

UnsetPublishedAt ensures that no value is present for PublishedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


