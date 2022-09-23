# \SDWANDeviceTemplateApi

All URIs are relative to *https://44.196.44.132*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DataserviceTemplateFeatureGet**](SDWANDeviceTemplateApi.md#DataserviceTemplateFeatureGet) | **Get** /dataservice/template/feature | Template Feature
[**DataserviceTemplateFeatureTypesGet**](SDWANDeviceTemplateApi.md#DataserviceTemplateFeatureTypesGet) | **Get** /dataservice/template/feature/types | Template Feature Type



## DataserviceTemplateFeatureGet

> DataserviceTemplateFeatureGet(ctx).XXSRFTOKEN(xXSRFTOKEN).Execute()

Template Feature

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
    resp, r, err := apiClient.SDWANDeviceTemplateApi.DataserviceTemplateFeatureGet(context.Background()).XXSRFTOKEN(xXSRFTOKEN).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SDWANDeviceTemplateApi.DataserviceTemplateFeatureGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDataserviceTemplateFeatureGetRequest struct via the builder pattern


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


## DataserviceTemplateFeatureTypesGet

> DataserviceTemplateFeatureTypesGet(ctx).XXSRFTOKEN(xXSRFTOKEN).Execute()

Template Feature Type

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
    resp, r, err := apiClient.SDWANDeviceTemplateApi.DataserviceTemplateFeatureTypesGet(context.Background()).XXSRFTOKEN(xXSRFTOKEN).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `SDWANDeviceTemplateApi.DataserviceTemplateFeatureTypesGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDataserviceTemplateFeatureTypesGetRequest struct via the builder pattern


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

