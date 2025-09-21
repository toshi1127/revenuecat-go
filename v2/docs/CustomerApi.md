# \CustomerAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateCustomer**](CustomerAPI.md#CreateCustomer) | **Post** /projects/{project_id}/customers | Create a customer
[**CreateVirtualCurrenciesTransaction**](CustomerAPI.md#CreateVirtualCurrenciesTransaction) | **Post** /projects/{project_id}/customers/{customer_id}/virtual_currencies/transactions | Create a virtual currencies transaction
[**DeleteCustomer**](CustomerAPI.md#DeleteCustomer) | **Delete** /projects/{project_id}/customers/{customer_id} | Delete a customer
[**GetCustomer**](CustomerAPI.md#GetCustomer) | **Get** /projects/{project_id}/customers/{customer_id} | Get a customer
[**ListCustomerActiveEntitlements**](CustomerAPI.md#ListCustomerActiveEntitlements) | **Get** /projects/{project_id}/customers/{customer_id}/active_entitlements | Get a list of customer&#39;s active entitlements
[**ListCustomerAliases**](CustomerAPI.md#ListCustomerAliases) | **Get** /projects/{project_id}/customers/{customer_id}/aliases | Get a list of the customer&#39;s aliases
[**ListCustomerAttributes**](CustomerAPI.md#ListCustomerAttributes) | **Get** /projects/{project_id}/customers/{customer_id}/attributes | Get a list of the customer&#39;s attributes
[**ListCustomers**](CustomerAPI.md#ListCustomers) | **Get** /projects/{project_id}/customers | Get a list of customers
[**ListPurchases**](CustomerAPI.md#ListPurchases) | **Get** /projects/{project_id}/customers/{customer_id}/purchases | Get a list of purchases associated with a customer
[**ListSubscriptions**](CustomerAPI.md#ListSubscriptions) | **Get** /projects/{project_id}/customers/{customer_id}/subscriptions | Get a list of subscriptions associated with a customer
[**ListVirtualCurrenciesBalances**](CustomerAPI.md#ListVirtualCurrenciesBalances) | **Get** /projects/{project_id}/customers/{customer_id}/virtual_currencies | Get a list of customer&#39;s virtual currencies balances
[**SetCustomerAttributes**](CustomerAPI.md#SetCustomerAttributes) | **Post** /projects/{project_id}/customers/{customer_id}/attributes | Set a customer&#39;s attributes
[**TransferCustomerData**](CustomerAPI.md#TransferCustomerData) | **Post** /projects/{project_id}/customers/{customer_id}/actions/transfer | Transfer customer&#39;s subscriptions and one-time purchases to another customer
[**UpdateVirtualCurrenciesBalance**](CustomerAPI.md#UpdateVirtualCurrenciesBalance) | **Post** /projects/{project_id}/customers/{customer_id}/virtual_currencies/update_balance | Update a virtual currencies balance without creating a transaction



## CreateCustomer

> Customer CreateCustomer(ctx, projectId).CreateCustomerRequest(createCustomerRequest).Execute()

Create a customer



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
	createCustomerRequest := *openapiclient.NewCreateCustomerRequest("19b8de26-77c1-49f1-aa18-019a391603e2") // CreateCustomerRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.CreateCustomer(context.Background(), projectId).CreateCustomerRequest(createCustomerRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.CreateCustomer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCustomer`: Customer
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.CreateCustomer`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateCustomerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createCustomerRequest** | [**CreateCustomerRequest**](CreateCustomerRequest.md) |  | 

### Return type

[**Customer**](Customer.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateVirtualCurrenciesTransaction

> ListVirtualCurrenciesBalances CreateVirtualCurrenciesTransaction(ctx, projectId, customerId).CreateVirtualCurrenciesTransactionRequest(createVirtualCurrenciesTransactionRequest).IdempotencyKey(idempotencyKey).IncludeEmptyBalances(includeEmptyBalances).Execute()

Create a virtual currencies transaction



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	createVirtualCurrenciesTransactionRequest := *openapiclient.NewCreateVirtualCurrenciesTransactionRequest(map[string]int32{"key": int32(123)}) // CreateVirtualCurrenciesTransactionRequest | 
	idempotencyKey := "1234-5678-9101-1121" // string | This is an optional idempotency key to ensure exactly once execution of the request. (optional)
	includeEmptyBalances := true // bool |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.CreateVirtualCurrenciesTransaction(context.Background(), projectId, customerId).CreateVirtualCurrenciesTransactionRequest(createVirtualCurrenciesTransactionRequest).IdempotencyKey(idempotencyKey).IncludeEmptyBalances(includeEmptyBalances).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.CreateVirtualCurrenciesTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateVirtualCurrenciesTransaction`: ListVirtualCurrenciesBalances
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.CreateVirtualCurrenciesTransaction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateVirtualCurrenciesTransactionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **createVirtualCurrenciesTransactionRequest** | [**CreateVirtualCurrenciesTransactionRequest**](CreateVirtualCurrenciesTransactionRequest.md) |  | 
 **idempotencyKey** | **string** | This is an optional idempotency key to ensure exactly once execution of the request. | 
 **includeEmptyBalances** | **bool** |  | 

### Return type

[**ListVirtualCurrenciesBalances**](ListVirtualCurrenciesBalances.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteCustomer

> DeletedObject DeleteCustomer(ctx, projectId, customerId).Execute()

Delete a customer



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.DeleteCustomer(context.Background(), projectId, customerId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.DeleteCustomer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteCustomer`: DeletedObject
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.DeleteCustomer`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteCustomerRequest struct via the builder pattern


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


## GetCustomer

> Customer GetCustomer(ctx, projectId, customerId).Expand(expand).Execute()

Get a customer



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	expand := []string{"attributes"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `attributes` (requires `customer_information:customers:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.GetCustomer(context.Background(), projectId, customerId).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.GetCustomer``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCustomer`: Customer
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.GetCustomer`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCustomerRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;attributes&#x60; (requires &#x60;customer_information:customers:read&#x60; permission). | 

### Return type

[**Customer**](Customer.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomerActiveEntitlements

> ListCustomerActiveEntitlements ListCustomerActiveEntitlements(ctx, projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of customer's active entitlements



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.ListCustomerActiveEntitlements(context.Background(), projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.ListCustomerActiveEntitlements``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomerActiveEntitlements`: ListCustomerActiveEntitlements
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.ListCustomerActiveEntitlements`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCustomerActiveEntitlementsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ListCustomerActiveEntitlements**](ListCustomerActiveEntitlements.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomerAliases

> ListCustomerAliases ListCustomerAliases(ctx, projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of the customer's aliases



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.ListCustomerAliases(context.Background(), projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.ListCustomerAliases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomerAliases`: ListCustomerAliases
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.ListCustomerAliases`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCustomerAliasesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ListCustomerAliases**](ListCustomerAliases.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomerAttributes

> ListCustomerAttributes ListCustomerAttributes(ctx, projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of the customer's attributes



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.ListCustomerAttributes(context.Background(), projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.ListCustomerAttributes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomerAttributes`: ListCustomerAttributes
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.ListCustomerAttributes`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCustomerAttributesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ListCustomerAttributes**](ListCustomerAttributes.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomers

> ListCustomers ListCustomers(ctx, projectId).StartingAfter(startingAfter).Limit(limit).Search(search).Execute()

Get a list of customers



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
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)
	search := "example@example.com" // string | Search term. Currently, only searching by email is supported (searching for exact matches in the $email attribute). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.ListCustomers(context.Background(), projectId).StartingAfter(startingAfter).Limit(limit).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.ListCustomers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomers`: ListCustomers
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.ListCustomers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCustomersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]
 **search** | **string** | Search term. Currently, only searching by email is supported (searching for exact matches in the $email attribute). | 

### Return type

[**ListCustomers**](ListCustomers.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPurchases

> ListPurchases ListPurchases(ctx, projectId, customerId).Environment(environment).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of purchases associated with a customer



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	environment := "production" // string |  (optional)
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.ListPurchases(context.Background(), projectId, customerId).Environment(environment).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.ListPurchases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPurchases`: ListPurchases
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.ListPurchases`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPurchasesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **environment** | **string** |  | 
 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

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


## ListSubscriptions

> ListSubscriptions ListSubscriptions(ctx, projectId, customerId).Environment(environment).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of subscriptions associated with a customer



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	environment := "production" // string |  (optional)
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.ListSubscriptions(context.Background(), projectId, customerId).Environment(environment).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.ListSubscriptions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSubscriptions`: ListSubscriptions
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.ListSubscriptions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiListSubscriptionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **environment** | **string** |  | 
 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

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


## ListVirtualCurrenciesBalances

> ListVirtualCurrenciesBalances ListVirtualCurrenciesBalances(ctx, projectId, customerId).IncludeEmptyBalances(includeEmptyBalances).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of customer's virtual currencies balances



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	includeEmptyBalances := true // bool |  (optional)
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.ListVirtualCurrenciesBalances(context.Background(), projectId, customerId).IncludeEmptyBalances(includeEmptyBalances).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.ListVirtualCurrenciesBalances``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListVirtualCurrenciesBalances`: ListVirtualCurrenciesBalances
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.ListVirtualCurrenciesBalances`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiListVirtualCurrenciesBalancesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **includeEmptyBalances** | **bool** |  | 
 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ListVirtualCurrenciesBalances**](ListVirtualCurrenciesBalances.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetCustomerAttributes

> ListCustomerAttributes SetCustomerAttributes(ctx, projectId, customerId).SetCustomerAttributesRequest(setCustomerAttributesRequest).Execute()

Set a customer's attributes



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	setCustomerAttributesRequest := *openapiclient.NewSetCustomerAttributesRequest([]openapiclient.SetCustomerAttributesRequestAttributesInner{*openapiclient.NewSetCustomerAttributesRequestAttributesInner(openapiclient.create_customer_request_attributes_inner_name{CustomerAttributeReservedName: openapiclient.CustomerAttributeReservedName("$ad")}, "Value_example")}) // SetCustomerAttributesRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.SetCustomerAttributes(context.Background(), projectId, customerId).SetCustomerAttributesRequest(setCustomerAttributesRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.SetCustomerAttributes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SetCustomerAttributes`: ListCustomerAttributes
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.SetCustomerAttributes`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetCustomerAttributesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **setCustomerAttributesRequest** | [**SetCustomerAttributesRequest**](SetCustomerAttributesRequest.md) |  | 

### Return type

[**ListCustomerAttributes**](ListCustomerAttributes.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TransferCustomerData

> Transfer TransferCustomerData(ctx, projectId, customerId).TransferCustomerDataRequest(transferCustomerDataRequest).Execute()

Transfer customer's subscriptions and one-time purchases to another customer



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	transferCustomerDataRequest := *openapiclient.NewTransferCustomerDataRequest("TargetCustomerId_example") // TransferCustomerDataRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.TransferCustomerData(context.Background(), projectId, customerId).TransferCustomerDataRequest(transferCustomerDataRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.TransferCustomerData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TransferCustomerData`: Transfer
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.TransferCustomerData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiTransferCustomerDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **transferCustomerDataRequest** | [**TransferCustomerDataRequest**](TransferCustomerDataRequest.md) |  | 

### Return type

[**Transfer**](Transfer.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateVirtualCurrenciesBalance

> ListVirtualCurrenciesBalances UpdateVirtualCurrenciesBalance(ctx, projectId, customerId).CreateVirtualCurrenciesTransactionRequest(createVirtualCurrenciesTransactionRequest).IdempotencyKey(idempotencyKey).IncludeEmptyBalances(includeEmptyBalances).Execute()

Update a virtual currencies balance without creating a transaction



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	createVirtualCurrenciesTransactionRequest := *openapiclient.NewCreateVirtualCurrenciesTransactionRequest(map[string]int32{"key": int32(123)}) // CreateVirtualCurrenciesTransactionRequest | 
	idempotencyKey := "1234-5678-9101-1121" // string | This is an optional idempotency key to ensure exactly once execution of the request. (optional)
	includeEmptyBalances := true // bool |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomerAPI.UpdateVirtualCurrenciesBalance(context.Background(), projectId, customerId).CreateVirtualCurrenciesTransactionRequest(createVirtualCurrenciesTransactionRequest).IdempotencyKey(idempotencyKey).IncludeEmptyBalances(includeEmptyBalances).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomerAPI.UpdateVirtualCurrenciesBalance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateVirtualCurrenciesBalance`: ListVirtualCurrenciesBalances
	fmt.Fprintf(os.Stdout, "Response from `CustomerAPI.UpdateVirtualCurrenciesBalance`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateVirtualCurrenciesBalanceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **createVirtualCurrenciesTransactionRequest** | [**CreateVirtualCurrenciesTransactionRequest**](CreateVirtualCurrenciesTransactionRequest.md) |  | 
 **idempotencyKey** | **string** | This is an optional idempotency key to ensure exactly once execution of the request. | 
 **includeEmptyBalances** | **bool** |  | 

### Return type

[**ListVirtualCurrenciesBalances**](ListVirtualCurrenciesBalances.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

