# AttachProductsToPackageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Products** | [**[]PackageProductIDAssociation**](PackageProductIDAssociation.md) | Product association list | 

## Methods

### NewAttachProductsToPackageRequest

`func NewAttachProductsToPackageRequest(products []PackageProductIDAssociation, ) *AttachProductsToPackageRequest`

NewAttachProductsToPackageRequest instantiates a new AttachProductsToPackageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAttachProductsToPackageRequestWithDefaults

`func NewAttachProductsToPackageRequestWithDefaults() *AttachProductsToPackageRequest`

NewAttachProductsToPackageRequestWithDefaults instantiates a new AttachProductsToPackageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProducts

`func (o *AttachProductsToPackageRequest) GetProducts() []PackageProductIDAssociation`

GetProducts returns the Products field if non-nil, zero value otherwise.

### GetProductsOk

`func (o *AttachProductsToPackageRequest) GetProductsOk() (*[]PackageProductIDAssociation, bool)`

GetProductsOk returns a tuple with the Products field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProducts

`func (o *AttachProductsToPackageRequest) SetProducts(v []PackageProductIDAssociation)`

SetProducts sets Products field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


