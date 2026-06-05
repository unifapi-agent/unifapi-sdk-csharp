# Unifapi.Sdk.Api.NewsApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**NewsSearchPost**](NewsApi.md#newssearchpost) | **POST** /news/search | Search News |

<a id="newssearchpost"></a>
# **NewsSearchPost**
> NewsSearchPost200Response NewsSearchPost (NewsSearchRequest? newsSearchRequest = null)

Search News

Run one live News search and receive the ranked news articles and top-stories blocks for a query, including title, publisher domain, snippet, image, and publish time.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class NewsSearchPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new NewsApi(config);
            var newsSearchRequest = new NewsSearchRequest?(); // NewsSearchRequest? |  (optional) 

            try
            {
                // Search News
                NewsSearchPost200Response result = apiInstance.NewsSearchPost(newsSearchRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling NewsApi.NewsSearchPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the NewsSearchPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search News
    ApiResponse<NewsSearchPost200Response> response = apiInstance.NewsSearchPostWithHttpInfo(newsSearchRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling NewsApi.NewsSearchPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **newsSearchRequest** | [**NewsSearchRequest?**](NewsSearchRequest?.md) |  | [optional]  |

### Return type

[**NewsSearchPost200Response**](NewsSearchPost200Response.md)

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

