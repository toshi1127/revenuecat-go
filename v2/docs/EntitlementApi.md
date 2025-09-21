# \EntitlementAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AttachProductsToEntitlement**](EntitlementAPI.md#AttachProductsToEntitlement) | **Post** /projects/{project_id}/entitlements/{entitlement_id}/actions/attach_products | Attach a set of products to an entitlement
[**CreateEntitlement**](EntitlementAPI.md#CreateEntitlement) | **Post** /projects/{project_id}/entitlements | Create an entitlement
[**DeleteEntitlement**](EntitlementAPI.md#DeleteEntitlement) | **Delete** /projects/{project_id}/entitlements/{entitlement_id} | Delete an entitlement
[**DetachProductsFromEntitlement**](EntitlementAPI.md#DetachProductsFromEntitlement) | **Post** /projects/{project_id}/entitlements/{entitlement_id}/actions/detach_products | Detach a set of product from an entitlement
[**GetEntitlement**](EntitlementAPI.md#GetEntitlement) | **Get** /projects/{project_id}/entitlements/{entitlement_id} | Get an entitlement
[**GetProductsFromEntitlement**](EntitlementAPI.md#GetProductsFromEntitlement) | **Get** /projects/{project_id}/entitlements/{entitlement_id}/products | Get a list of products attached to a given entitlement
[**ListEntitlements**](EntitlementAPI.md#ListEntitlements) | **Get** /projects/{project_id}/entitlements | Get a list of entitlements
[**UpdateEntitlement**](EntitlementAPI.md#UpdateEntitlement) | **Post** /projects/{project_id}/entitlements/{entitlement_id} | Update an entitlement



## AttachProductsToEntitlement

> Entitlement AttachProductsToEntitlement(ctx, projectId, entitlementId).AttachProductsToEntitlementRequest(attachProductsToEntitlementRequest).Execute()

Attach a set of products to an entitlement



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	entitlementId := "entla1b2c3d4e5" // string | ID of the entitlement
	attachProductsToEntitlementRequest := *openapiclient.NewAttachProductsToEntitlementRequest([]string{"prod1a2b3c4d5e"}) // AttachProductsToEntitlementRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.AttachProductsToEntitlement(context.Background(), projectId, entitlementId).AttachProductsToEntitlementRequest(attachProductsToEntitlementRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.AttachProductsToEntitlement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AttachProductsToEntitlement`: Entitlement
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.AttachProductsToEntitlement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**entitlementId** | **string** | ID of the entitlement | 

### Other Parameters

Other parameters are passed through a pointer to a apiAttachProductsToEntitlementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **attachProductsToEntitlementRequest** | [**AttachProductsToEntitlementRequest**](AttachProductsToEntitlementRequest.md) |  | 

### Return type

[**Entitlement**](Entitlement.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateEntitlement

> Entitlement CreateEntitlement(ctx, projectId).CreateEntitlementRequest(createEntitlementRequest).Execute()

Create an entitlement



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	createEntitlementRequest := *openapiclient.NewCreateEntitlementRequest("premium", "Premium access to all features") // CreateEntitlementRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.CreateEntitlement(context.Background(), projectId).CreateEntitlementRequest(createEntitlementRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.CreateEntitlement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEntitlement`: Entitlement
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.CreateEntitlement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateEntitlementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createEntitlementRequest** | [**CreateEntitlementRequest**](CreateEntitlementRequest.md) |  | 

### Return type

[**Entitlement**](Entitlement.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteEntitlement

> DeletedObject DeleteEntitlement(ctx, projectId, entitlementId).Execute()

Delete an entitlement



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	entitlementId := "entla1b2c3d4e5" // string | ID of the entitlement

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.DeleteEntitlement(context.Background(), projectId, entitlementId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.DeleteEntitlement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteEntitlement`: DeletedObject
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.DeleteEntitlement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**entitlementId** | **string** | ID of the entitlement | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEntitlementRequest struct via the builder pattern


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


## DetachProductsFromEntitlement

> Entitlement DetachProductsFromEntitlement(ctx, projectId, entitlementId).DetachProductsFromEntitlementRequest(detachProductsFromEntitlementRequest).Execute()

Detach a set of product from an entitlement



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	entitlementId := "entla1b2c3d4e5" // string | ID of the entitlement
	detachProductsFromEntitlementRequest := *openapiclient.NewDetachProductsFromEntitlementRequest([]string{"prod1a2b3c4d5e"}) // DetachProductsFromEntitlementRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.DetachProductsFromEntitlement(context.Background(), projectId, entitlementId).DetachProductsFromEntitlementRequest(detachProductsFromEntitlementRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.DetachProductsFromEntitlement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DetachProductsFromEntitlement`: Entitlement
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.DetachProductsFromEntitlement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**entitlementId** | **string** | ID of the entitlement | 

### Other Parameters

Other parameters are passed through a pointer to a apiDetachProductsFromEntitlementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **detachProductsFromEntitlementRequest** | [**DetachProductsFromEntitlementRequest**](DetachProductsFromEntitlementRequest.md) |  | 

### Return type

[**Entitlement**](Entitlement.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEntitlement

> Entitlement GetEntitlement(ctx, projectId, entitlementId).Expand(expand).Execute()

Get an entitlement



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	entitlementId := "entla1b2c3d4e5" // string | ID of the entitlement
	expand := []string{"product"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `product` (requires `project_configuration:products:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.GetEntitlement(context.Background(), projectId, entitlementId).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.GetEntitlement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEntitlement`: Entitlement
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.GetEntitlement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**entitlementId** | **string** | ID of the entitlement | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEntitlementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;product&#x60; (requires &#x60;project_configuration:products:read&#x60; permission). | 

### Return type

[**Entitlement**](Entitlement.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProductsFromEntitlement

> ProductsFromEntitlement GetProductsFromEntitlement(ctx, projectId, entitlementId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of products attached to a given entitlement



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	entitlementId := "entla1b2c3d4e5" // string | ID of the entitlement
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.GetProductsFromEntitlement(context.Background(), projectId, entitlementId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.GetProductsFromEntitlement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProductsFromEntitlement`: ProductsFromEntitlement
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.GetProductsFromEntitlement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**entitlementId** | **string** | ID of the entitlement | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProductsFromEntitlementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ProductsFromEntitlement**](ProductsFromEntitlement.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListEntitlements

> ListEntitlements ListEntitlements(ctx, projectId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()

Get a list of entitlements



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)
	expand := []string{"items.product"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `items.product` (requires `project_configuration:products:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.ListEntitlements(context.Background(), projectId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.ListEntitlements``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEntitlements`: ListEntitlements
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.ListEntitlements`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiListEntitlementsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]
 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;items.product&#x60; (requires &#x60;project_configuration:products:read&#x60; permission). | 

### Return type

[**ListEntitlements**](ListEntitlements.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEntitlement

> Entitlement UpdateEntitlement(ctx, projectId, entitlementId).UpdateEntitlementRequest(updateEntitlementRequest).Execute()

Update an entitlement



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/toshi1127/go-revenuecat/v2"
)

func main() {
	projectId := "proj1ab2c3d4" // string | ID of the project
	entitlementId := "entla1b2c3d4e5" // string | ID of the entitlement
	updateEntitlementRequest := *openapiclient.NewUpdateEntitlementRequest("Premium") // UpdateEntitlementRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntitlementAPI.UpdateEntitlement(context.Background(), projectId, entitlementId).UpdateEntitlementRequest(updateEntitlementRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntitlementAPI.UpdateEntitlement``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEntitlement`: Entitlement
	fmt.Fprintf(os.Stdout, "Response from `EntitlementAPI.UpdateEntitlement`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**entitlementId** | **string** | ID of the entitlement | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEntitlementRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateEntitlementRequest** | [**UpdateEntitlementRequest**](UpdateEntitlementRequest.md) |  | 

### Return type

[**Entitlement**](Entitlement.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

