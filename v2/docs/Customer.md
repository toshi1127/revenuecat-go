# Customer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Object** | **string** | String representing the object&#39;s type. Objects of the same type share the same value. | 
**Id** | **string** |  | 
**ProjectId** | **string** | ID of the project to which the customer belongs | 
**FirstSeenAt** | **int64** | The first time the customer was seen | 
**LastSeenAt** | **NullableInt64** | The last time the customer was seen | 
**LastSeenAppVersion** | **NullableString** | The last app version the customer was seen on | 
**LastSeenCountry** | **NullableString** | The last country the customer was seen in | 
**LastSeenPlatform** | **NullableString** | The last platform the customer was seen on | 
**LastSeenPlatformVersion** | **NullableString** | The last platform version the customer was seen on | 
**ActiveEntitlements** | Pointer to [**CustomerActiveEntitlements**](CustomerActiveEntitlements.md) |  | [optional] 
**Experiment** | Pointer to [**NullableExperimentEnrollment**](ExperimentEnrollment.md) |  | [optional] 
**Attributes** | Pointer to [**CustomerAttributes**](CustomerAttributes.md) |  | [optional] 

## Methods

### NewCustomer

`func NewCustomer(object string, id string, projectId string, firstSeenAt int64, lastSeenAt NullableInt64, lastSeenAppVersion NullableString, lastSeenCountry NullableString, lastSeenPlatform NullableString, lastSeenPlatformVersion NullableString, ) *Customer`

NewCustomer instantiates a new Customer object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCustomerWithDefaults

`func NewCustomerWithDefaults() *Customer`

NewCustomerWithDefaults instantiates a new Customer object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetObject

`func (o *Customer) GetObject() string`

GetObject returns the Object field if non-nil, zero value otherwise.

### GetObjectOk

`func (o *Customer) GetObjectOk() (*string, bool)`

GetObjectOk returns a tuple with the Object field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetObject

`func (o *Customer) SetObject(v string)`

SetObject sets Object field to given value.


### GetId

`func (o *Customer) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Customer) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Customer) SetId(v string)`

SetId sets Id field to given value.


### GetProjectId

`func (o *Customer) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *Customer) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *Customer) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.


### GetFirstSeenAt

`func (o *Customer) GetFirstSeenAt() int64`

GetFirstSeenAt returns the FirstSeenAt field if non-nil, zero value otherwise.

### GetFirstSeenAtOk

`func (o *Customer) GetFirstSeenAtOk() (*int64, bool)`

GetFirstSeenAtOk returns a tuple with the FirstSeenAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstSeenAt

`func (o *Customer) SetFirstSeenAt(v int64)`

SetFirstSeenAt sets FirstSeenAt field to given value.


### GetLastSeenAt

`func (o *Customer) GetLastSeenAt() int64`

GetLastSeenAt returns the LastSeenAt field if non-nil, zero value otherwise.

### GetLastSeenAtOk

`func (o *Customer) GetLastSeenAtOk() (*int64, bool)`

GetLastSeenAtOk returns a tuple with the LastSeenAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenAt

`func (o *Customer) SetLastSeenAt(v int64)`

SetLastSeenAt sets LastSeenAt field to given value.


### SetLastSeenAtNil

`func (o *Customer) SetLastSeenAtNil(b bool)`

 SetLastSeenAtNil sets the value for LastSeenAt to be an explicit nil

### UnsetLastSeenAt
`func (o *Customer) UnsetLastSeenAt()`

UnsetLastSeenAt ensures that no value is present for LastSeenAt, not even an explicit nil
### GetLastSeenAppVersion

`func (o *Customer) GetLastSeenAppVersion() string`

GetLastSeenAppVersion returns the LastSeenAppVersion field if non-nil, zero value otherwise.

### GetLastSeenAppVersionOk

`func (o *Customer) GetLastSeenAppVersionOk() (*string, bool)`

GetLastSeenAppVersionOk returns a tuple with the LastSeenAppVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenAppVersion

`func (o *Customer) SetLastSeenAppVersion(v string)`

SetLastSeenAppVersion sets LastSeenAppVersion field to given value.


### SetLastSeenAppVersionNil

`func (o *Customer) SetLastSeenAppVersionNil(b bool)`

 SetLastSeenAppVersionNil sets the value for LastSeenAppVersion to be an explicit nil

### UnsetLastSeenAppVersion
`func (o *Customer) UnsetLastSeenAppVersion()`

UnsetLastSeenAppVersion ensures that no value is present for LastSeenAppVersion, not even an explicit nil
### GetLastSeenCountry

`func (o *Customer) GetLastSeenCountry() string`

GetLastSeenCountry returns the LastSeenCountry field if non-nil, zero value otherwise.

### GetLastSeenCountryOk

`func (o *Customer) GetLastSeenCountryOk() (*string, bool)`

GetLastSeenCountryOk returns a tuple with the LastSeenCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenCountry

`func (o *Customer) SetLastSeenCountry(v string)`

SetLastSeenCountry sets LastSeenCountry field to given value.


### SetLastSeenCountryNil

`func (o *Customer) SetLastSeenCountryNil(b bool)`

 SetLastSeenCountryNil sets the value for LastSeenCountry to be an explicit nil

### UnsetLastSeenCountry
`func (o *Customer) UnsetLastSeenCountry()`

UnsetLastSeenCountry ensures that no value is present for LastSeenCountry, not even an explicit nil
### GetLastSeenPlatform

`func (o *Customer) GetLastSeenPlatform() string`

GetLastSeenPlatform returns the LastSeenPlatform field if non-nil, zero value otherwise.

### GetLastSeenPlatformOk

`func (o *Customer) GetLastSeenPlatformOk() (*string, bool)`

GetLastSeenPlatformOk returns a tuple with the LastSeenPlatform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenPlatform

`func (o *Customer) SetLastSeenPlatform(v string)`

SetLastSeenPlatform sets LastSeenPlatform field to given value.


### SetLastSeenPlatformNil

`func (o *Customer) SetLastSeenPlatformNil(b bool)`

 SetLastSeenPlatformNil sets the value for LastSeenPlatform to be an explicit nil

### UnsetLastSeenPlatform
`func (o *Customer) UnsetLastSeenPlatform()`

UnsetLastSeenPlatform ensures that no value is present for LastSeenPlatform, not even an explicit nil
### GetLastSeenPlatformVersion

`func (o *Customer) GetLastSeenPlatformVersion() string`

GetLastSeenPlatformVersion returns the LastSeenPlatformVersion field if non-nil, zero value otherwise.

### GetLastSeenPlatformVersionOk

`func (o *Customer) GetLastSeenPlatformVersionOk() (*string, bool)`

GetLastSeenPlatformVersionOk returns a tuple with the LastSeenPlatformVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSeenPlatformVersion

`func (o *Customer) SetLastSeenPlatformVersion(v string)`

SetLastSeenPlatformVersion sets LastSeenPlatformVersion field to given value.


### SetLastSeenPlatformVersionNil

`func (o *Customer) SetLastSeenPlatformVersionNil(b bool)`

 SetLastSeenPlatformVersionNil sets the value for LastSeenPlatformVersion to be an explicit nil

### UnsetLastSeenPlatformVersion
`func (o *Customer) UnsetLastSeenPlatformVersion()`

UnsetLastSeenPlatformVersion ensures that no value is present for LastSeenPlatformVersion, not even an explicit nil
### GetActiveEntitlements

`func (o *Customer) GetActiveEntitlements() CustomerActiveEntitlements`

GetActiveEntitlements returns the ActiveEntitlements field if non-nil, zero value otherwise.

### GetActiveEntitlementsOk

`func (o *Customer) GetActiveEntitlementsOk() (*CustomerActiveEntitlements, bool)`

GetActiveEntitlementsOk returns a tuple with the ActiveEntitlements field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveEntitlements

`func (o *Customer) SetActiveEntitlements(v CustomerActiveEntitlements)`

SetActiveEntitlements sets ActiveEntitlements field to given value.

### HasActiveEntitlements

`func (o *Customer) HasActiveEntitlements() bool`

HasActiveEntitlements returns a boolean if a field has been set.

### GetExperiment

`func (o *Customer) GetExperiment() ExperimentEnrollment`

GetExperiment returns the Experiment field if non-nil, zero value otherwise.

### GetExperimentOk

`func (o *Customer) GetExperimentOk() (*ExperimentEnrollment, bool)`

GetExperimentOk returns a tuple with the Experiment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExperiment

`func (o *Customer) SetExperiment(v ExperimentEnrollment)`

SetExperiment sets Experiment field to given value.

### HasExperiment

`func (o *Customer) HasExperiment() bool`

HasExperiment returns a boolean if a field has been set.

### SetExperimentNil

`func (o *Customer) SetExperimentNil(b bool)`

 SetExperimentNil sets the value for Experiment to be an explicit nil

### UnsetExperiment
`func (o *Customer) UnsetExperiment()`

UnsetExperiment ensures that no value is present for Experiment, not even an explicit nil
### GetAttributes

`func (o *Customer) GetAttributes() CustomerAttributes`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *Customer) GetAttributesOk() (*CustomerAttributes, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *Customer) SetAttributes(v CustomerAttributes)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *Customer) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


