# \ChartsMetricsAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetOverviewMetrics**](ChartsMetricsAPI.md#GetOverviewMetrics) | **Get** /projects/{project_id}/metrics/overview | Get overview metrics for a project



## GetOverviewMetrics

> OverviewMetrics GetOverviewMetrics(ctx, projectId).Currency(currency).Execute()

Get overview metrics for a project



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
	currency := "EUR" // string | ISO 4217 currency code (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ChartsMetricsAPI.GetOverviewMetrics(context.Background(), projectId).Currency(currency).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ChartsMetricsAPI.GetOverviewMetrics``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOverviewMetrics`: OverviewMetrics
	fmt.Fprintf(os.Stdout, "Response from `ChartsMetricsAPI.GetOverviewMetrics`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetOverviewMetricsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **currency** | **string** | ISO 4217 currency code | 

### Return type

[**OverviewMetrics**](OverviewMetrics.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

