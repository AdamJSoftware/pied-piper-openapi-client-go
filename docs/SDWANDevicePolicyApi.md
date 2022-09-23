# \SDWANDevicePolicyApi

All URIs are relative to *https://44.196.44.132*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DataserviceTemplatePolicyListGet**](SDWANDevicePolicyApi.md#DataserviceTemplatePolicyListGet) | **Get** /dataservice/template/policy/list | Policy List
[**DataserviceTemplatePolicyVedgeDevicesGet**](SDWANDevicePolicyApi.md#DataserviceTemplatePolicyVedgeDevicesGet) | **Get** /dataservice/template/policy/vedge/devices | vEdge Template Policy



## DataserviceTemplatePolicyListGet

> DataserviceTemplatePolicyListGet(ctx).XXSRFTOKEN(xXSRFTOKEN).Execute()

Policy List

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    xXSRFTOKEN := "{{X-XSRF-TOKEN}}" // string |  (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.SDWANDevicePolicyApi.DataserviceTemplatePolicyListGet(context.Background()).XXSRFTOKEN(xXSRFTOKEN).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SDWANDevicePolicyApi.DataserviceTemplatePolicyListGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDataserviceTemplatePolicyListGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xXSRFTOKEN** | **string** |  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DataserviceTemplatePolicyVedgeDevicesGet

> DataserviceTemplatePolicyVedgeDevicesGet(ctx).Execute()

vEdge Template Policy

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.SDWANDevicePolicyApi.DataserviceTemplatePolicyVedgeDevicesGet(context.Background()).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SDWANDevicePolicyApi.DataserviceTemplatePolicyVedgeDevicesGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDataserviceTemplatePolicyVedgeDevicesGetRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

