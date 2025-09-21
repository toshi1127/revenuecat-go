# \AppAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateApp**](AppAPI.md#CreateApp) | **Post** /projects/{project_id}/apps | Create an App
[**DeleteApp**](AppAPI.md#DeleteApp) | **Delete** /projects/{project_id}/apps/{app_id} | Delete an app
[**GetApp**](AppAPI.md#GetApp) | **Get** /projects/{project_id}/apps/{app_id} | Get an app
[**GetAppStorekitConfig**](AppAPI.md#GetAppStorekitConfig) | **Get** /projects/{project_id}/apps/{app_id}/store_kit_config | Get the StoreKit configuration for an app
[**ListAppPublicApiKeys**](AppAPI.md#ListAppPublicApiKeys) | **Get** /projects/{project_id}/apps/{app_id}/public_api_keys | Get a list of the public API keys of an app
[**ListApps**](AppAPI.md#ListApps) | **Get** /projects/{project_id}/apps | Get a list of apps
[**UpdateApp**](AppAPI.md#UpdateApp) | **Post** /projects/{project_id}/apps/{app_id} | Update an app



## CreateApp

> App CreateApp(ctx, projectId).AppCreate(appCreate).Execute()

Create an App



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
	appCreate := map[string][]openapiclient.AppCreate{ ... } // AppCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppAPI.CreateApp(context.Background(), projectId).AppCreate(appCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppAPI.CreateApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateApp`: App
	fmt.Fprintf(os.Stdout, "Response from `AppAPI.CreateApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateAppRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **appCreate** | [**AppCreate**](AppCreate.md) |  | 

### Return type

[**App**](App.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteApp

> DeletedObject DeleteApp(ctx, projectId, appId).Execute()

Delete an app



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
	appId := "app1ab2c3d4" // string | ID of the app

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppAPI.DeleteApp(context.Background(), projectId, appId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppAPI.DeleteApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteApp`: DeletedObject
	fmt.Fprintf(os.Stdout, "Response from `AppAPI.DeleteApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**appId** | **string** | ID of the app | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAppRequest struct via the builder pattern


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


## GetApp

> App GetApp(ctx, projectId, appId).Execute()

Get an app



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
	appId := "app1ab2c3d4" // string | ID of the app

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppAPI.GetApp(context.Background(), projectId, appId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppAPI.GetApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetApp`: App
	fmt.Fprintf(os.Stdout, "Response from `AppAPI.GetApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**appId** | **string** | ID of the app | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAppRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**App**](App.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAppStorekitConfig

> StoreKitConfigFile GetAppStorekitConfig(ctx, projectId, appId).Execute()

Get the StoreKit configuration for an app



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
	appId := "app1ab2c3d4" // string | ID of the app

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppAPI.GetAppStorekitConfig(context.Background(), projectId, appId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppAPI.GetAppStorekitConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAppStorekitConfig`: StoreKitConfigFile
	fmt.Fprintf(os.Stdout, "Response from `AppAPI.GetAppStorekitConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**appId** | **string** | ID of the app | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAppStorekitConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**StoreKitConfigFile**](StoreKitConfigFile.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAppPublicApiKeys

> ListPublicApiKeys ListAppPublicApiKeys(ctx, projectId, appId).Execute()

Get a list of the public API keys of an app



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
	appId := "app1ab2c3d4" // string | ID of the app

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppAPI.ListAppPublicApiKeys(context.Background(), projectId, appId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppAPI.ListAppPublicApiKeys``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAppPublicApiKeys`: ListPublicApiKeys
	fmt.Fprintf(os.Stdout, "Response from `AppAPI.ListAppPublicApiKeys`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**appId** | **string** | ID of the app | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAppPublicApiKeysRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ListPublicApiKeys**](ListPublicApiKeys.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListApps

> ListApps ListApps(ctx, projectId).StartingAfter(startingAfter).Limit(limit).Execute()

Get a list of apps



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppAPI.ListApps(context.Background(), projectId).StartingAfter(startingAfter).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppAPI.ListApps``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListApps`: ListApps
	fmt.Fprintf(os.Stdout, "Response from `AppAPI.ListApps`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAppsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]

### Return type

[**ListApps**](ListApps.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApp

> App UpdateApp(ctx, projectId, appId).UpdateAppRequest(updateAppRequest).Execute()

Update an app



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
	appId := "app1ab2c3d4" // string | ID of the app
	updateAppRequest := *openapiclient.NewUpdateAppRequest() // UpdateAppRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AppAPI.UpdateApp(context.Background(), projectId, appId).UpdateAppRequest(updateAppRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AppAPI.UpdateApp``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApp`: App
	fmt.Fprintf(os.Stdout, "Response from `AppAPI.UpdateApp`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**appId** | **string** | ID of the app | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAppRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateAppRequest** | [**UpdateAppRequest**](UpdateAppRequest.md) |  | 

### Return type

[**App**](App.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

