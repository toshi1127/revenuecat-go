# \OfferingAPI

All URIs are relative to *https://api.revenuecat.com/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateOffering**](OfferingAPI.md#CreateOffering) | **Post** /projects/{project_id}/offerings | Create an offering
[**DeleteOffering**](OfferingAPI.md#DeleteOffering) | **Delete** /projects/{project_id}/offerings/{offering_id} | Delete an offering and its attached packages
[**GetOffering**](OfferingAPI.md#GetOffering) | **Get** /projects/{project_id}/offerings/{offering_id} | Get an offering
[**ListOfferings**](OfferingAPI.md#ListOfferings) | **Get** /projects/{project_id}/offerings | Get a list of offerings
[**UpdateOffering**](OfferingAPI.md#UpdateOffering) | **Post** /projects/{project_id}/offerings/{offering_id} | Update an offering



## CreateOffering

> Offering CreateOffering(ctx, projectId).CreateOfferingRequest(createOfferingRequest).Execute()

Create an offering



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
	createOfferingRequest := *openapiclient.NewCreateOfferingRequest("default", "The standard set of packages") // CreateOfferingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OfferingAPI.CreateOffering(context.Background(), projectId).CreateOfferingRequest(createOfferingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OfferingAPI.CreateOffering``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateOffering`: Offering
	fmt.Fprintf(os.Stdout, "Response from `OfferingAPI.CreateOffering`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateOfferingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createOfferingRequest** | [**CreateOfferingRequest**](CreateOfferingRequest.md) |  | 

### Return type

[**Offering**](Offering.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteOffering

> DeletedObject DeleteOffering(ctx, projectId, offeringId).Execute()

Delete an offering and its attached packages



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OfferingAPI.DeleteOffering(context.Background(), projectId, offeringId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OfferingAPI.DeleteOffering``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteOffering`: DeletedObject
	fmt.Fprintf(os.Stdout, "Response from `OfferingAPI.DeleteOffering`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**offeringId** | **string** | ID of the offering | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteOfferingRequest struct via the builder pattern


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


## GetOffering

> Offering GetOffering(ctx, projectId, offeringId).Expand(expand).Execute()

Get an offering



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
	expand := []string{"package"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `package` (requires `project_configuration:packages:read` permission), `package.product` (requires `project_configuration:products:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OfferingAPI.GetOffering(context.Background(), projectId, offeringId).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OfferingAPI.GetOffering``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOffering`: Offering
	fmt.Fprintf(os.Stdout, "Response from `OfferingAPI.GetOffering`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**offeringId** | **string** | ID of the offering | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetOfferingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;package&#x60; (requires &#x60;project_configuration:packages:read&#x60; permission), &#x60;package.product&#x60; (requires &#x60;project_configuration:products:read&#x60; permission). | 

### Return type

[**Offering**](Offering.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListOfferings

> ListOfferings ListOfferings(ctx, projectId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()

Get a list of offerings



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
	expand := []string{"items.package"} // []string | Specifies which fields in the response should be expanded.  Accepted values are: `items.package` (requires `project_configuration:packages:read` permission), `items.package.product` (requires `project_configuration:products:read` permission). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OfferingAPI.ListOfferings(context.Background(), projectId).StartingAfter(startingAfter).Limit(limit).Expand(expand).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OfferingAPI.ListOfferings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListOfferings`: ListOfferings
	fmt.Fprintf(os.Stdout, "Response from `OfferingAPI.ListOfferings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 

### Other Parameters

Other parameters are passed through a pointer to a apiListOfferingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startingAfter** | **string** |  | 
 **limit** | **int32** |  | [default to 20]
 **expand** | **[]string** | Specifies which fields in the response should be expanded.  Accepted values are: &#x60;items.package&#x60; (requires &#x60;project_configuration:packages:read&#x60; permission), &#x60;items.package.product&#x60; (requires &#x60;project_configuration:products:read&#x60; permission). | 

### Return type

[**ListOfferings**](ListOfferings.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateOffering

> Offering UpdateOffering(ctx, projectId, offeringId).UpdateOfferingRequest(updateOfferingRequest).Execute()

Update an offering



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
	updateOfferingRequest := *openapiclient.NewUpdateOfferingRequest() // UpdateOfferingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OfferingAPI.UpdateOffering(context.Background(), projectId, offeringId).UpdateOfferingRequest(updateOfferingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OfferingAPI.UpdateOffering``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateOffering`: Offering
	fmt.Fprintf(os.Stdout, "Response from `OfferingAPI.UpdateOffering`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | ID of the project | 
**offeringId** | **string** | ID of the offering | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateOfferingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateOfferingRequest** | [**UpdateOfferingRequest**](UpdateOfferingRequest.md) |  | 

### Return type

[**Offering**](Offering.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

