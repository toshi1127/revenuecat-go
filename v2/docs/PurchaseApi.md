# \PurchaseAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetPurchase**](PurchaseAPI.md#GetPurchase) | **Get** /projects/{project_id}/purchases/{purchase_id} | Get a purchase
[**ListPurchaseEntitlements**](PurchaseAPI.md#ListPurchaseEntitlements) | **Get** /projects/{project_id}/purchases/{purchase_id}/entitlements | Get a list of entitlements associated with a purchase
[**RefundPurchase**](PurchaseAPI.md#RefundPurchase) | **Post** /projects/{project_id}/purchases/{purchase_id}/actions/refund | Refund a Web Billing purchase
[**SearchPurchases**](PurchaseAPI.md#SearchPurchases) | **Get** /projects/{project_id}/purchases | Search one-time purchases by store purchase identifier



## GetPurchase

> Purchase GetPurchase(ctx, projectId, purchaseId).Execute()

Get a purchase



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
	purchaseId := "purc1a2b3c4d5e" // string | ID of the purchase

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PurchaseAPI.GetPurchase(context.Background(), projectId, purchaseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PurchaseAPI.GetPurchase``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPurchase`: Purchase
	fmt.Fprintf(os.Stdout, "Response from `PurchaseAPI.GetPurchase`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**purchaseId** | **string** | ID of the purchase | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPurchaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Purchase**](Purchase.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPurchaseEntitlements

> ListEntitlements ListPurchaseEntitlements(ctx, projectId, purchaseId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of entitlements associated with a purchase



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
	purchaseId := "purc1a2b3c4d5e" // string | ID of the purchase
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PurchaseAPI.ListPurchaseEntitlements(context.Background(), projectId, purchaseId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PurchaseAPI.ListPurchaseEntitlements``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPurchaseEntitlements`: ListEntitlements
	fmt.Fprintf(os.Stdout, "Response from `PurchaseAPI.ListPurchaseEntitlements`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**purchaseId** | **string** | ID of the purchase | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPurchaseEntitlementsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

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


## RefundPurchase

> Purchase RefundPurchase(ctx, projectId, purchaseId).Execute()

Refund a Web Billing purchase



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
	purchaseId := "purc1a2b3c4d5e" // string | ID of the purchase

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PurchaseAPI.RefundPurchase(context.Background(), projectId, purchaseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PurchaseAPI.RefundPurchase``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RefundPurchase`: Purchase
	fmt.Fprintf(os.Stdout, "Response from `PurchaseAPI.RefundPurchase`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**purchaseId** | **string** | ID of the purchase | 

### Other Parameters

Other parameters are passed through a pointer to a apiRefundPurchaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Purchase**](Purchase.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchPurchases

> ListPurchases SearchPurchases(ctx, projectId).StorePurchaseIdentifier(storePurchaseIdentifier).Execute()

Search one-time purchases by store purchase identifier



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
	storePurchaseIdentifier := "9aJscueFTxLPZXXo-AlBTkI0OnFXR2qiH14C1aqWnOT=:3:11" // string | Store ID associated with the one-time purchase.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PurchaseAPI.SearchPurchases(context.Background(), projectId).StorePurchaseIdentifier(storePurchaseIdentifier).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PurchaseAPI.SearchPurchases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchPurchases`: ListPurchases
	fmt.Fprintf(os.Stdout, "Response from `PurchaseAPI.SearchPurchases`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiSearchPurchasesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **storePurchaseIdentifier** | **string** | Store ID associated with the one-time purchase. | 

### Return type

[**ListPurchases**](ListPurchases.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

