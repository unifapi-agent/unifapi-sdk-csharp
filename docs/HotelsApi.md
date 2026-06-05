# Unifapi.Sdk.Api.HotelsApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**HotelsInfoPost**](HotelsApi.md#hotelsinfopost) | **POST** /hotels/info | Get Hotels detail |
| [**HotelsSearchPost**](HotelsApi.md#hotelssearchpost) | **POST** /hotels/search | Search Hotels |

<a id="hotelsinfopost"></a>
# **HotelsInfoPost**
> HotelsInfoPost200Response HotelsInfoPost (HotelInfoRequest? hotelInfoRequest = null)

Get Hotels detail

Run one live Hotels detail lookup for a hotel id from /hotels/search and receive the full profile, including class rating, address, phone, description, guest reviews, images, and prices.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HotelsInfoPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HotelsApi(config);
            var hotelInfoRequest = new HotelInfoRequest?(); // HotelInfoRequest? |  (optional) 

            try
            {
                // Get Hotels detail
                HotelsInfoPost200Response result = apiInstance.HotelsInfoPost(hotelInfoRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HotelsApi.HotelsInfoPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HotelsInfoPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get Hotels detail
    ApiResponse<HotelsInfoPost200Response> response = apiInstance.HotelsInfoPostWithHttpInfo(hotelInfoRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HotelsApi.HotelsInfoPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **hotelInfoRequest** | [**HotelInfoRequest?**](HotelInfoRequest?.md) |  | [optional]  |

### Return type

[**HotelsInfoPost200Response**](HotelsInfoPost200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Validation or invalid-id error |  -  |
| **401** | Missing, invalid, disabled, revoked, or expired UnifAPI API key |  -  |
| **402** | Insufficient workspace credits |  -  |
| **404** | Resource not found |  -  |
| **429** | Rate limited |  -  |
| **500** | Internal error |  -  |
| **502** | Source error |  -  |
| **503** | Source unavailable |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="hotelssearchpost"></a>
# **HotelsSearchPost**
> HotelsSearchPost200Response HotelsSearchPost (HotelSearchRequest? hotelSearchRequest = null)

Search Hotels

Run one live Hotels search and receive ranked hotel listings for a location and stay dates, including hotel id, class rating, guest reviews, and nightly prices. Pass a hotel id to /hotels/info for full details.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HotelsSearchPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HotelsApi(config);
            var hotelSearchRequest = new HotelSearchRequest?(); // HotelSearchRequest? |  (optional) 

            try
            {
                // Search Hotels
                HotelsSearchPost200Response result = apiInstance.HotelsSearchPost(hotelSearchRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HotelsApi.HotelsSearchPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HotelsSearchPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search Hotels
    ApiResponse<HotelsSearchPost200Response> response = apiInstance.HotelsSearchPostWithHttpInfo(hotelSearchRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HotelsApi.HotelsSearchPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **hotelSearchRequest** | [**HotelSearchRequest?**](HotelSearchRequest?.md) |  | [optional]  |

### Return type

[**HotelsSearchPost200Response**](HotelsSearchPost200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Validation or invalid-id error |  -  |
| **401** | Missing, invalid, disabled, revoked, or expired UnifAPI API key |  -  |
| **402** | Insufficient workspace credits |  -  |
| **404** | Resource not found |  -  |
| **429** | Rate limited |  -  |
| **500** | Internal error |  -  |
| **502** | Source error |  -  |
| **503** | Source unavailable |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

