# OverviewMetric

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** | Id of the overview metric | 
**Name** | **string** | Display name of the overview metric | 
**Description** | **string** | Description of the overview metric | 
**Unit** | **string** | Unit of the overview metric | 
**Period** | **string** | Length of time during which metric data is collected in ISO 8601 format. Zero period means metric data was collected now | 
**Value** | **float32** | Value of the overview metric | 
**LastUpdatedAt** | **NullableInt64** | Last time the overview metric was updated in ms since epoch | 
**LastUpdatedAtIso8601** | **NullableTime** | Last time the overview metric was updated datetime in ISO 8601 format | 

## Methods

### NewOverviewMetric

`func NewOverviewMetric(object string, id string, name string, description string, unit string, period string, value float32, lastUpdatedAt NullableInt64, lastUpdatedAtIso8601 NullableTime, ) *OverviewMetric`

NewOverviewMetric instantiates a new OverviewMetric object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOverviewMetricWithDefaults

`func NewOverviewMetricWithDefaults() *OverviewMetric`

NewOverviewMetricWithDefaults instantiates a new OverviewMetric object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *OverviewMetric) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *OverviewMetric) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *OverviewMetric) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *OverviewMetric) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *OverviewMetric) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *OverviewMetric) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *OverviewMetric) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *OverviewMetric) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *OverviewMetric) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *OverviewMetric) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *OverviewMetric) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *OverviewMetric) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetUnit

`func (o *OverviewMetric) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *OverviewMetric) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *OverviewMetric) SetUnit(v string)`

SetUnit sets Unit field to given value.


### GetPeriod

`func (o *OverviewMetric) GetPeriod() string`

GetPeriod returns the Period field if non-nil, zero value otherwise.

### GetPeriodOk

`func (o *OverviewMetric) GetPeriodOk() (*string, bool)`

GetPeriodOk returns a tuple with the Period field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPeriod

`func (o *OverviewMetric) SetPeriod(v string)`

SetPeriod sets Period field to given value.


### GetValue

`func (o *OverviewMetric) GetValue() float32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *OverviewMetric) GetValueOk() (*float32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *OverviewMetric) SetValue(v float32)`

SetValue sets Value field to given value.


### GetLastUpdatedAt

`func (o *OverviewMetric) GetLastUpdatedAt() int64`

GetLastUpdatedAt returns the LastUpdatedAt field if non-nil, zero value otherwise.

### GetLastUpdatedAtOk

`func (o *OverviewMetric) GetLastUpdatedAtOk() (*int64, bool)`

GetLastUpdatedAtOk returns a tuple with the LastUpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUpdatedAt

`func (o *OverviewMetric) SetLastUpdatedAt(v int64)`

SetLastUpdatedAt sets LastUpdatedAt field to given value.


### SetLastUpdatedAtNil

`func (o *OverviewMetric) SetLastUpdatedAtNil(b bool)`

 SetLastUpdatedAtNil sets the value for LastUpdatedAt to be an explicit nil

### UnsetLastUpdatedAt
`func (o *OverviewMetric) UnsetLastUpdatedAt()`

UnsetLastUpdatedAt ensures that no value is present for LastUpdatedAt, not even an explicit nil
### GetLastUpdatedAtIso8601

`func (o *OverviewMetric) GetLastUpdatedAtIso8601() time.Time`

GetLastUpdatedAtIso8601 returns the LastUpdatedAtIso8601 field if non-nil, zero value otherwise.

### GetLastUpdatedAtIso8601Ok

`func (o *OverviewMetric) GetLastUpdatedAtIso8601Ok() (*time.Time, bool)`

GetLastUpdatedAtIso8601Ok returns a tuple with the LastUpdatedAtIso8601 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUpdatedAtIso8601

`func (o *OverviewMetric) SetLastUpdatedAtIso8601(v time.Time)`

SetLastUpdatedAtIso8601 sets LastUpdatedAtIso8601 field to given value.


### SetLastUpdatedAtIso8601Nil

`func (o *OverviewMetric) SetLastUpdatedAtIso8601Nil(b bool)`

 SetLastUpdatedAtIso8601Nil sets the value for LastUpdatedAtIso8601 to be an explicit nil

### UnsetLastUpdatedAtIso8601
`func (o *OverviewMetric) UnsetLastUpdatedAtIso8601()`

UnsetLastUpdatedAtIso8601 ensures that no value is present for LastUpdatedAtIso8601, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


