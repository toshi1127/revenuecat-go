# OverviewMetrics

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Metrics** | [**[]OverviewMetric**](OverviewMetric.md) | Details about each overview metric. | 

## Methods

### NewOverviewMetrics

`func NewOverviewMetrics(object string, metrics []OverviewMetric, ) *OverviewMetrics`

NewOverviewMetrics instantiates a new OverviewMetrics object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOverviewMetricsWithDefaults

`func NewOverviewMetricsWithDefaults() *OverviewMetrics`

NewOverviewMetricsWithDefaults instantiates a new OverviewMetrics object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *OverviewMetrics) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *OverviewMetrics) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *OverviewMetrics) SetObject(v string)`

SetObject sets Object field to given value.


### GetMetrics

`func (o *OverviewMetrics) GetMetrics() []OverviewMetric`

GetMetrics returns the Metrics field if non-nil, zero value otherwise.

### GetMetricsOk

`func (o *OverviewMetrics) GetMetricsOk() (*[]OverviewMetric, bool)`

GetMetricsOk returns a tuple with the Metrics field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetrics

`func (o *OverviewMetrics) SetMetrics(v []OverviewMetric)`

SetMetrics sets Metrics field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


