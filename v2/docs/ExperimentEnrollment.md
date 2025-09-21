# ExperimentEnrollment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** |  | 
**Name** | **string** |  | 
**Variant** | **string** | The variant of the Experiment that the Customer was or is assigned to, where &#39;a&#39; represents the Control, and &#39;b&#39; represents the Treatment. | 

## Methods

### NewExperimentEnrollment

`func NewExperimentEnrollment(object string, id string, name string, variant string, ) *ExperimentEnrollment`

NewExperimentEnrollment instantiates a new ExperimentEnrollment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExperimentEnrollmentWithDefaults

`func NewExperimentEnrollmentWithDefaults() *ExperimentEnrollment`

NewExperimentEnrollmentWithDefaults instantiates a new ExperimentEnrollment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *ExperimentEnrollment) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *ExperimentEnrollment) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *ExperimentEnrollment) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *ExperimentEnrollment) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ExperimentEnrollment) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ExperimentEnrollment) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *ExperimentEnrollment) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ExperimentEnrollment) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ExperimentEnrollment) SetName(v string)`

SetName sets Name field to given value.


### GetVariant

`func (o *ExperimentEnrollment) GetVariant() string`

GetVariant returns the Variant field if non-nil, zero value otherwise.

### GetVariantOk

`func (o *ExperimentEnrollment) GetVariantOk() (*string, bool)`

GetVariantOk returns a tuple with the Variant field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariant

`func (o *ExperimentEnrollment) SetVariant(v string)`

SetVariant sets Variant field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


