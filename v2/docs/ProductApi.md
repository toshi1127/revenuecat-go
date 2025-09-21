# \ProductAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateProduct**](ProductAPI.md#CreateProduct) | **Post** /projects/{project_id}/products | Create a product
[**CreateProductInStore**](ProductAPI.md#CreateProductInStore) | **Post** /projects/{project_id}/products/{product_id}/create_in_store | Push a product to the store
[**DeleteProduct**](ProductAPI.md#DeleteProduct) | **Delete** /projects/{project_id}/products/{product_id} | Delete a product
[**GetProduct**](ProductAPI.md#GetProduct) | **Get** /projects/{project_id}/products/{product_id} | Get a product
[**ListProducts**](ProductAPI.md#ListProducts) | **Get** /projects/{project_id}/products | Get a list of products



## CreateProduct

> Product CreateProduct(ctx, projectId).CreateProductRequest(createProductRequest).Execute()

Create a product



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
	createProductRequest := *openapiclient.NewCreateProductRequest("com.revenuecat.magicweather.monthly", "app1a2b3c4", openapiclient.ProductType("subscription")) // CreateProductRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProductAPI.CreateProduct(context.Background(), projectId).CreateProductRequest(createProductRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProductAPI.CreateProduct``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateProduct`: Product
	fmt.Fprintf(os.Stdout, "Response from `ProductAPI.CreateProduct`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateProductRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createProductRequest** | [**CreateProductRequest**](CreateProductRequest.md) |  | 

### Return type

[**Product**](Product.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateProductInStore

> CreateProductInStore201Response CreateProductInStore(ctx, projectId, productId).CreateProductInStoreRequest(createProductInStoreRequest).Execute()

Push a product to the store



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
	productId := "prod1a2b3c4d5" // string | ID of the product
	createProductInStoreRequest := *openapiclient.NewCreateProductInStoreRequest() // CreateProductInStoreRequest | Store-specific information. Only required for subscription products. For in-app purchase products, send an empty body or omit the request body entirely.  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProductAPI.CreateProductInStore(context.Background(), projectId, productId).CreateProductInStoreRequest(createProductInStoreRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProductAPI.CreateProductInStore``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateProductInStore`: CreateProductInStore201Response
	fmt.Fprintf(os.Stdout, "Response from `ProductAPI.CreateProductInStore`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**productId** | **string** | ID of the product | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateProductInStoreRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **createProductInStoreRequest** | [**CreateProductInStoreRequest**](CreateProductInStoreRequest.md) | Store-specific information. Only required for subscription products. For in-app purchase products, send an empty body or omit the request body entirely.  | 

### Return type

[**CreateProductInStore201Response**](CreateProductInStore201Response.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteProduct

> DeletedObject DeleteProduct(ctx, projectId, productId).Execute()

Delete a product



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
	productId := "prod1a2b3c4d5" // string | ID of the product

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProductAPI.DeleteProduct(context.Background(), projectId, productId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProductAPI.DeleteProduct``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteProduct`: DeletedObject
	fmt.Fprintf(os.Stdout, "Response from `ProductAPI.DeleteProduct`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**productId** | **string** | ID of the product | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteProductRequest struct via the builder pattern


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


## GetProduct

> Product GetProduct(ctx, projectId, productId).Expand(expand).Execute()

Get a product



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
	productId := "prod1a2b3c4d5" // string | ID of the product
	expand := []string{"app"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `app` (requires `project_configuration:apps:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProductAPI.GetProduct(context.Background(), projectId, productId).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProductAPI.GetProduct``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProduct`: Product
	fmt.Fprintf(os.Stdout, "Response from `ProductAPI.GetProduct`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**productId** | **string** | ID of the product | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetProductRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;app&#x60; (requires &#x60;project_configuration:apps:read&#x60; permission). | 

### Return type

[**Product**](Product.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListProducts

> ListProducts ListProducts(ctx, projectId).AppId(appId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()

Get a list of products



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
	appId := "app1a2b3c4" // string | This is an optional query parameter to get a list of products of a given entitlement associated with a particular app (optional)
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)
	expand := []string{"items.app"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `items.app` (requires `project_configuration:apps:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ProductAPI.ListProducts(context.Background(), projectId).AppId(appId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ProductAPI.ListProducts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListProducts`: ListProducts
	fmt.Fprintf(os.Stdout, "Response from `ProductAPI.ListProducts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiListProductsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **appId** | **string** | This is an optional query parameter to get a list of products of a given entitlement associated with a particular app | 
 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]
 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;items.app&#x60; (requires &#x60;project_configuration:apps:read&#x60; permission). | 

### Return type

[**ListProducts**](ListProducts.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

