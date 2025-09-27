# RevenueCat Go SDK

[![Go Version](https://img.shields.io/badge/go-1.23+-blue.svg)](https://golang.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

A Go SDK for the RevenueCat Developer API v2. This library provides type-safe Go bindings for RevenueCat's REST API, enabling you to manage subscriptions, customers, products, and more from your Go applications.

## Features

- **Complete API Coverage**: Full support for RevenueCat Developer API v2
- **Comprehensive Models**: All RevenueCat data models as Go structs
- **Auto-generated**: Generated from official OpenAPI specification

## Installation

```bash
go get github.com/toshi1127/revenuecat-go/v2
```

## Quick Start

```go
package main

import (
    "context"
    "fmt"
    "log"
    
    "github.com/toshi1127/revenuecat-go/v2"
)

func main() {
    // Initialize the client
    config := v2.NewConfiguration()
    config.Servers = []v2.ServerConfiguration{
        {
            URL: "https://api.revenuecat.com/v2",
        },
    }
    
    // Set your API key
    config.DefaultHeader["Authorization"] = "Bearer YOUR_API_KEY"
    
    client := v2.NewAPIClient(config)
    
    // Example: List projects
    ctx := context.Background()
    projects, response, err := client.ProjectAPI.ListProjects(ctx).Execute()
    if err != nil {
        log.Fatalf("Error listing projects: %v", err)
    }
    
    fmt.Printf("Found %d projects\n", len(projects.Data))
}
```

## API Coverage

This SDK supports all RevenueCat API v2 endpoints:

- **Apps**: Manage your applications across different platforms
- **Customers**: Customer management and attributes
- **Products**: Product catalog management
- **Subscriptions**: Subscription lifecycle management
- **Purchases**: Purchase tracking and validation
- **Entitlements**: Entitlement management
- **Offerings**: Offering and package management
- **Paywalls**: Paywall configuration
- **Charts & Metrics**: Analytics and reporting
- **Invoices**: Invoice management

## Development

### Prerequisites

- Go 1.23 or later
- Docker (for code generation)

### Generate Go Structs from OpenAPI

The Go structs are generated from the official RevenueCat OpenAPI specification:

```bash
make openapigen
```

This command uses Docker to run the OpenAPI Generator and update the Go code from the latest API specification.

### Project Structure

```
v2/
├── api/              # API client methods
├── model_*.go        # Data models and structs
├── client.go         # HTTP client implementation
├── configuration.go  # Client configuration
└── docs/            # Generated documentation
```

## Usage Examples

### Customer Management

```go
// Create a customer
createReq := v2.NewCreateCustomerRequest()
createReq.Data = v2.NewCreateCustomerRequestData()
createReq.Data.Attributes = []v2.CreateCustomerRequestAttributesInner{
    {
        Name:  v2.PtrString("email"),
        Value: v2.PtrString("customer@example.com"),
    },
}

customer, _, err := client.CustomerAPI.CreateCustomer(ctx).CreateCustomerRequest(*createReq).Execute()
```

### Product Management

```go
// List products
products, _, err := client.ProductAPI.ListProducts(ctx).Execute()
if err != nil {
    log.Fatal(err)
}

for _, product := range products.Data {
    fmt.Printf("Product: %s\n", *product.Attributes.Identifier)
}
```

### Subscription Management

```go
// Get customer subscriptions
subscriptions, _, err := client.SubscriptionAPI.ListSubscriptions(ctx).
    CustomerId("customer_id").
    Execute()
```

## Configuration

The client can be configured with various options:

```go
config := v2.NewConfiguration()
config.Servers = []v2.ServerConfiguration{
    {URL: "https://api.revenuecat.com/v2"},
}
config.DefaultHeader["Authorization"] = "Bearer YOUR_API_KEY"
config.Debug = true // Enable debug logging
```

## Error Handling

The SDK provides detailed error information:

```go
_, response, err := client.CustomerAPI.GetCustomer(ctx, "customer_id").Execute()
if err != nil {
    if response != nil {
        fmt.Printf("HTTP Status: %d\n", response.StatusCode)
        fmt.Printf("Response Body: %s\n", string(response.Body))
    }
    log.Fatal(err)
}
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Links

- [RevenueCat Documentation](https://www.revenuecat.com/docs/)
- [RevenueCat API Reference](https://www.revenuecat.com/docs/api-v2)
- [OpenAPI Specification](https://www.revenuecat.com/docs/redocusaurus/plugin-redoc-0.yaml)

## Support

For issues related to this Go SDK, please open an issue in this repository.

For RevenueCat API questions, please refer to the [RevenueCat Support](https://support.revenuecat.com/).