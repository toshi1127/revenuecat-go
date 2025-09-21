# \PackageAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AttachProductsToPackage**](PackageAPI.md#AttachProductsToPackage) | **Post** /projects/{project_id}/packages/{package_id}/actions/attach_products | Attach a set of products to a package
[**CreatePackages**](PackageAPI.md#CreatePackages) | **Post** /projects/{project_id}/offerings/{offering_id}/packages | Create a package
[**DeletePackageFromOffering**](PackageAPI.md#DeletePackageFromOffering) | **Delete** /projects/{project_id}/packages/{package_id} | Delete a package
[**DetachProductsFromPackage**](PackageAPI.md#DetachProductsFromPackage) | **Post** /projects/{project_id}/packages/{package_id}/actions/detach_products | Detach a set of products from a package
[**GetPackage**](PackageAPI.md#GetPackage) | **Get** /projects/{project_id}/packages/{package_id} | Get a package
[**GetProductsFromPackage**](PackageAPI.md#GetProductsFromPackage) | **Get** /projects/{project_id}/packages/{package_id}/products | Get a list of products attached to a given package of an offering
[**ListPackages**](PackageAPI.md#ListPackages) | **Get** /projects/{project_id}/offerings/{offering_id}/packages | Get a list of packages in an offering
[**UpdatePackage**](PackageAPI.md#UpdatePackage) | **Post** /projects/{project_id}/packages/{package_id} | Update a package



## AttachProductsToPackage

> Package AttachProductsToPackage(ctx, projectId, packageId).AttachProductsToPackageRequest(attachProductsToPackageRequest).Execute()

Attach a set of products to a package



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	packageId := "pkge1a2b3c4d5" // string | ID of the package
	attachProductsToPackageRequest := *openapiclient.NewAttachProductsToPackageRequest([]openapiclient.PackageProductIDAssociation{*openapiclient.NewPackageProductIDAssociation("ProductId_example", openapiclient.EligibilityCriteria("all"))}) // AttachProductsToPackageRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.AttachProductsToPackage(context.Background(), projectId, packageId).AttachProductsToPackageRequest(attachProductsToPackageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.AttachProductsToPackage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AttachProductsToPackage`: Package
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.AttachProductsToPackage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**packageId** | **string** | ID of the package | 

### Other Parameters

Other parameters are passed through a pointer to a apiAttachProductsToPackageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **attachProductsToPackageRequest** | [**AttachProductsToPackageRequest**](AttachProductsToPackageRequest.md) |  | 

### Return type

[**Package**](Package.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreatePackages

> Package CreatePackages(ctx, projectId, offeringId).CreatePackagesRequest(createPackagesRequest).Execute()

Create a package



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	offeringId := "ofrnge1a2b3c4d5" // string | ID of the offering
	createPackagesRequest := *openapiclient.NewCreatePackagesRequest("monthly", "monthly with one-week trial") // CreatePackagesRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.CreatePackages(context.Background(), projectId, offeringId).CreatePackagesRequest(createPackagesRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.CreatePackages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePackages`: Package
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.CreatePackages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**offeringId** | **string** | ID of the offering | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreatePackagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **createPackagesRequest** | [**CreatePackagesRequest**](CreatePackagesRequest.md) |  | 

### Return type

[**Package**](Package.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeletePackageFromOffering

> DeletedObject DeletePackageFromOffering(ctx, projectId, packageId).Execute()

Delete a package



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	packageId := "pkge1a2b3c4d5" // string | ID of the package

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.DeletePackageFromOffering(context.Background(), projectId, packageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.DeletePackageFromOffering``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeletePackageFromOffering`: DeletedObject
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.DeletePackageFromOffering`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**packageId** | **string** | ID of the package | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeletePackageFromOfferingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DeletedObject**](DeletedObject.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DetachProductsFromPackage

> Package DetachProductsFromPackage(ctx, projectId, packageId).DetachProductsFromPackageRequest(detachProductsFromPackageRequest).Execute()

Detach a set of products from a package



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	packageId := "pkge1a2b3c4d5" // string | ID of the package
	detachProductsFromPackageRequest := *openapiclient.NewDetachProductsFromPackageRequest([]string{"prod1a2b3c4d5e"}) // DetachProductsFromPackageRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.DetachProductsFromPackage(context.Background(), projectId, packageId).DetachProductsFromPackageRequest(detachProductsFromPackageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.DetachProductsFromPackage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DetachProductsFromPackage`: Package
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.DetachProductsFromPackage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**packageId** | **string** | ID of the package | 

### Other Parameters

Other parameters are passed through a pointer to a apiDetachProductsFromPackageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **detachProductsFromPackageRequest** | [**DetachProductsFromPackageRequest**](DetachProductsFromPackageRequest.md) |  | 

### Return type

[**Package**](Package.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPackage

> Package GetPackage(ctx, projectId, packageId).Expand(expand).Execute()

Get a package



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	packageId := "pkge1a2b3c4d5" // string | ID of the package
	expand := []string{"product"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `product` (requires `project_configuration:products:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.GetPackage(context.Background(), projectId, packageId).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.GetPackage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPackage`: Package
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.GetPackage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**packageId** | **string** | ID of the package | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPackageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;product&#x60; (requires &#x60;project_configuration:products:read&#x60; permission). | 

### Return type

[**Package**](Package.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProductsFromPackage

> ProductsFromPackage GetProductsFromPackage(ctx, projectId, packageId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of products attached to a given package of an offering



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	packageId := "pkge1a2b3c4d5" // string | ID of the package
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.GetProductsFromPackage(context.Background(), projectId, packageId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.GetProductsFromPackage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProductsFromPackage`: ProductsFromPackage
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.GetProductsFromPackage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**packageId** | **string** | ID of the package | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProductsFromPackageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ProductsFromPackage**](ProductsFromPackage.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPackages

> ListPackages ListPackages(ctx, projectId, offeringId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()

Get a list of packages in an offering



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	offeringId := "ofrnge1a2b3c4d5" // string | ID of the offering
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)
	expand := []string{"items.product"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `items.product` (requires `project_configuration:products:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.ListPackages(context.Background(), projectId, offeringId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.ListPackages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPackages`: ListPackages
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.ListPackages`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**offeringId** | **string** | ID of the offering | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPackagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]
 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;items.product&#x60; (requires &#x60;project_configuration:products:read&#x60; permission). | 

### Return type

[**ListPackages**](ListPackages.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdatePackage

> Package UpdatePackage(ctx, projectId, packageId).UpdatePackageRequest(updatePackageRequest).Execute()

Update a package



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	packageId := "pkge1a2b3c4d5" // string | ID of the package
	updatePackageRequest := *openapiclient.NewUpdatePackageRequest() // UpdatePackageRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PackageAPI.UpdatePackage(context.Background(), projectId, packageId).UpdatePackageRequest(updatePackageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PackageAPI.UpdatePackage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdatePackage`: Package
	fmt.Fprintf(os.Stdout, "Response from `PackageAPI.UpdatePackage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**packageId** | **string** | ID of the package | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdatePackageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updatePackageRequest** | [**UpdatePackageRequest**](UpdatePackageRequest.md) |  | 

### Return type

[**Package**](Package.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

