# \SubscriptionAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelSubscription**](SubscriptionAPI.md#CancelSubscription) | **Post** /projects/{project_id}/subscriptions/{subscription_id}/actions/cancel | Cancel an active Web Billing subscription
[**GetAuthorizedSubscriptionManagementUrl**](SubscriptionAPI.md#GetAuthorizedSubscriptionManagementUrl) | **Get** /projects/{project_id}/subscriptions/{subscription_id}/authenticated_management_url | Get an authenticated Web Billing customer portal URL
[**GetPlayStoreSubscriptionTransactions**](SubscriptionAPI.md#GetPlayStoreSubscriptionTransactions) | **Get** /projects/{project_id}/subscriptions/{subscription_id}/transactions | Get a Play Store subscription&#39;s transactions
[**GetSubscription**](SubscriptionAPI.md#GetSubscription) | **Get** /projects/{project_id}/subscriptions/{subscription_id} | Get a subscription
[**ListSubscriptionEntitlements**](SubscriptionAPI.md#ListSubscriptionEntitlements) | **Get** /projects/{project_id}/subscriptions/{subscription_id}/entitlements | Get a list of entitlements associated with a subscription
[**RefundPlayStoreSubscriptionTransaction**](SubscriptionAPI.md#RefundPlayStoreSubscriptionTransaction) | **Post** /projects/{project_id}/subscriptions/{subscription_id}/transactions/{transaction_id}/actions/refund | Refund a Play Store subscription&#39;s transaction
[**RefundSubscription**](SubscriptionAPI.md#RefundSubscription) | **Post** /projects/{project_id}/subscriptions/{subscription_id}/actions/refund | Refund an active Web Billing subscription
[**SearchSubscriptions**](SubscriptionAPI.md#SearchSubscriptions) | **Get** /projects/{project_id}/subscriptions | Search subscriptions by store subscription identifier



## CancelSubscription

> Subscription CancelSubscription(ctx, projectId, subscriptionId).Execute()

Cancel an active Web Billing subscription



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
	subscriptionId := "sub1a2b3c4d5e" // string | ID of the subscription

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.CancelSubscription(context.Background(), projectId, subscriptionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.CancelSubscription``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelSubscription`: Subscription
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.CancelSubscription`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**subscriptionId** | **string** | ID of the subscription | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelSubscriptionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Subscription**](Subscription.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAuthorizedSubscriptionManagementUrl

> AuthenticatedManagementUrl GetAuthorizedSubscriptionManagementUrl(ctx, projectId, subscriptionId).Execute()

Get an authenticated Web Billing customer portal URL



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
	subscriptionId := "sub1a2b3c4d5e" // string | ID of the subscription

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.GetAuthorizedSubscriptionManagementUrl(context.Background(), projectId, subscriptionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.GetAuthorizedSubscriptionManagementUrl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAuthorizedSubscriptionManagementUrl`: AuthenticatedManagementUrl
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.GetAuthorizedSubscriptionManagementUrl`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**subscriptionId** | **string** | ID of the subscription | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAuthorizedSubscriptionManagementUrlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**AuthenticatedManagementUrl**](AuthenticatedManagementUrl.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPlayStoreSubscriptionTransactions

> ListSubscriptionTransaction GetPlayStoreSubscriptionTransactions(ctx, projectId, subscriptionId).Execute()

Get a Play Store subscription's transactions



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
	subscriptionId := "sub1a2b3c4d5e" // string | ID of the subscription

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.GetPlayStoreSubscriptionTransactions(context.Background(), projectId, subscriptionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.GetPlayStoreSubscriptionTransactions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPlayStoreSubscriptionTransactions`: ListSubscriptionTransaction
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.GetPlayStoreSubscriptionTransactions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**subscriptionId** | **string** | ID of the subscription | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPlayStoreSubscriptionTransactionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ListSubscriptionTransaction**](ListSubscriptionTransaction.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSubscription

> Subscription GetSubscription(ctx, projectId, subscriptionId).Execute()

Get a subscription



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
	subscriptionId := "sub1a2b3c4d5e" // string | ID of the subscription

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.GetSubscription(context.Background(), projectId, subscriptionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.GetSubscription``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSubscription`: Subscription
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.GetSubscription`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**subscriptionId** | **string** | ID of the subscription | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSubscriptionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Subscription**](Subscription.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSubscriptionEntitlements

> ListEntitlements ListSubscriptionEntitlements(ctx, projectId, subscriptionId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of entitlements associated with a subscription



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
	subscriptionId := "sub1a2b3c4d5e" // string | ID of the subscription
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.ListSubscriptionEntitlements(context.Background(), projectId, subscriptionId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.ListSubscriptionEntitlements``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSubscriptionEntitlements`: ListEntitlements
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.ListSubscriptionEntitlements`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**subscriptionId** | **string** | ID of the subscription | 

### Other Parameters

Other parameters are passed through a pointer to a apiListSubscriptionEntitlementsRequest struct via the builder pattern


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


## RefundPlayStoreSubscriptionTransaction

> SubscriptionTransaction RefundPlayStoreSubscriptionTransaction(ctx, projectId, subscriptionId, transactionId).Execute()

Refund a Play Store subscription's transaction



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
	subscriptionId := "sub1a2b3c4d5e" // string | ID of the subscription
	transactionId := "GPA.000-000-000-000" // string | Identifier of the transaction in the store

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.RefundPlayStoreSubscriptionTransaction(context.Background(), projectId, subscriptionId, transactionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.RefundPlayStoreSubscriptionTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RefundPlayStoreSubscriptionTransaction`: SubscriptionTransaction
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.RefundPlayStoreSubscriptionTransaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**subscriptionId** | **string** | ID of the subscription | 
**transactionId** | **string** | Identifier of the transaction in the store | 

### Other Parameters

Other parameters are passed through a pointer to a apiRefundPlayStoreSubscriptionTransactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**SubscriptionTransaction**](SubscriptionTransaction.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RefundSubscription

> Subscription RefundSubscription(ctx, projectId, subscriptionId).Execute()

Refund an active Web Billing subscription



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
	subscriptionId := "sub1a2b3c4d5e" // string | ID of the subscription

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.RefundSubscription(context.Background(), projectId, subscriptionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.RefundSubscription``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RefundSubscription`: Subscription
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.RefundSubscription`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**subscriptionId** | **string** | ID of the subscription | 

### Other Parameters

Other parameters are passed through a pointer to a apiRefundSubscriptionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**Subscription**](Subscription.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchSubscriptions

> ListSubscriptions SearchSubscriptions(ctx, projectId).StoreSubscriptionIdentifier(storeSubscriptionIdentifier).Execute()

Search subscriptions by store subscription identifier



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
	storeSubscriptionIdentifier := "9aJscueFTxLPZXXo-AlBTkI0OnFXR2qiH14C1aqWnOT=:3:11..8" // string | Store ID associated with the subscription for the current or next period.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubscriptionAPI.SearchSubscriptions(context.Background(), projectId).StoreSubscriptionIdentifier(storeSubscriptionIdentifier).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubscriptionAPI.SearchSubscriptions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchSubscriptions`: ListSubscriptions
	fmt.Fprintf(os.Stdout, "Response from `SubscriptionAPI.SearchSubscriptions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiSearchSubscriptionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **storeSubscriptionIdentifier** | **string** | Store ID associated with the subscription for the current or next period. | 

### Return type

[**ListSubscriptions**](ListSubscriptions.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

