# \InvoiceAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetInvoice**](InvoiceAPI.md#GetInvoice) | **Get** /projects/{project_id}/customers/{customer_id}/invoices/{invoice_id}/file | Get an invoice
[**ListCustomerInvoices**](InvoiceAPI.md#ListCustomerInvoices) | **Get** /projects/{project_id}/customers/{customer_id}/invoices | Get a list of the customer&#39;s invoices



## GetInvoice

> GetInvoice(ctx, projectId, customerId, invoiceId).Execute()

Get an invoice



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	invoiceId := "rcbin1a2b3c4d5e" // string | ID of the invoice

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.InvoiceAPI.GetInvoice(context.Background(), projectId, customerId, invoiceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoiceAPI.GetInvoice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 
**invoiceId** | **string** | ID of the invoice | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetInvoiceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

 (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomerInvoices

> ListCustomerInvoices ListCustomerInvoices(ctx, projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of the customer's invoices



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
	customerId := "19b8de26-77c1-49f1-aa18-019a391603e2" // string | ID of the customer
	startingAfter := "ent12354" // string |  (optional)
	limit := int32(10) // int32 |  (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InvoiceAPI.ListCustomerInvoices(context.Background(), projectId, customerId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InvoiceAPI.ListCustomerInvoices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomerInvoices`: ListCustomerInvoices
	fmt.Fprintf(os.Stdout, "Response from `InvoiceAPI.ListCustomerInvoices`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**customerId** | **string** | ID of the customer | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCustomerInvoicesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ListCustomerInvoices**](ListCustomerInvoices.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

