# Unifapi.Sdk.Api.BrowserApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**BrowserHtmlPost**](BrowserApi.md#browserhtmlpost) | **POST** /browser/html | Render a page to HTML |
| [**BrowserLinksPost**](BrowserApi.md#browserlinkspost) | **POST** /browser/links | Extract links from a page |
| [**BrowserMarkdownPost**](BrowserApi.md#browsermarkdownpost) | **POST** /browser/markdown | Render a page to Markdown |
| [**BrowserScreenshotPost**](BrowserApi.md#browserscreenshotpost) | **POST** /browser/screenshot | Capture a page screenshot |

<a id="browserhtmlpost"></a>
# **BrowserHtmlPost**
> BrowserHtmlPost200Response BrowserHtmlPost (BrowserHtmlRequest? browserHtmlRequest = null)

Render a page to HTML

Render a URL in a headless browser and return the fully rendered HTML after JavaScript execution — use it to read meta tags, structured data, and content that only appears after client-side rendering.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class BrowserHtmlPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new BrowserApi(config);
            var browserHtmlRequest = new BrowserHtmlRequest?(); // BrowserHtmlRequest? |  (optional) 

            try
            {
                // Render a page to HTML
                BrowserHtmlPost200Response result = apiInstance.BrowserHtmlPost(browserHtmlRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BrowserApi.BrowserHtmlPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BrowserHtmlPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Render a page to HTML
    ApiResponse<BrowserHtmlPost200Response> response = apiInstance.BrowserHtmlPostWithHttpInfo(browserHtmlRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BrowserApi.BrowserHtmlPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **browserHtmlRequest** | [**BrowserHtmlRequest?**](BrowserHtmlRequest?.md) |  | [optional]  |

### Return type

[**BrowserHtmlPost200Response**](BrowserHtmlPost200Response.md)

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

<a id="browserlinkspost"></a>
# **BrowserLinksPost**
> BrowserLinksPost200Response BrowserLinksPost (BrowserLinksRequest? browserLinksRequest = null)

Extract links from a page

Render a URL in a headless browser and return every link on the page as absolute URLs, including links injected by JavaScript. Optionally restrict to visible links or same-domain links for internal-link and broken-link audits.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class BrowserLinksPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new BrowserApi(config);
            var browserLinksRequest = new BrowserLinksRequest?(); // BrowserLinksRequest? |  (optional) 

            try
            {
                // Extract links from a page
                BrowserLinksPost200Response result = apiInstance.BrowserLinksPost(browserLinksRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BrowserApi.BrowserLinksPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BrowserLinksPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Extract links from a page
    ApiResponse<BrowserLinksPost200Response> response = apiInstance.BrowserLinksPostWithHttpInfo(browserLinksRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BrowserApi.BrowserLinksPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **browserLinksRequest** | [**BrowserLinksRequest?**](BrowserLinksRequest?.md) |  | [optional]  |

### Return type

[**BrowserLinksPost200Response**](BrowserLinksPost200Response.md)

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

<a id="browsermarkdownpost"></a>
# **BrowserMarkdownPost**
> BrowserMarkdownPost200Response BrowserMarkdownPost (BrowserMarkdownRequest? browserMarkdownRequest = null)

Render a page to Markdown

Render a URL in a headless browser (running JavaScript) and return the page as clean Markdown — ideal for content analysis, summarization, and feeding pages to language models.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class BrowserMarkdownPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new BrowserApi(config);
            var browserMarkdownRequest = new BrowserMarkdownRequest?(); // BrowserMarkdownRequest? |  (optional) 

            try
            {
                // Render a page to Markdown
                BrowserMarkdownPost200Response result = apiInstance.BrowserMarkdownPost(browserMarkdownRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BrowserApi.BrowserMarkdownPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BrowserMarkdownPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Render a page to Markdown
    ApiResponse<BrowserMarkdownPost200Response> response = apiInstance.BrowserMarkdownPostWithHttpInfo(browserMarkdownRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BrowserApi.BrowserMarkdownPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **browserMarkdownRequest** | [**BrowserMarkdownRequest?**](BrowserMarkdownRequest?.md) |  | [optional]  |

### Return type

[**BrowserMarkdownPost200Response**](BrowserMarkdownPost200Response.md)

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

<a id="browserscreenshotpost"></a>
# **BrowserScreenshotPost**
> BrowserScreenshotPost200Response BrowserScreenshotPost (BrowserScreenshotRequest? browserScreenshotRequest = null)

Capture a page screenshot

Render a URL in a headless browser and capture a screenshot, returned as a base64-encoded image. Control the viewport, capture the full scrollable page, target a CSS selector, and choose png, jpeg, or webp output.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class BrowserScreenshotPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new BrowserApi(config);
            var browserScreenshotRequest = new BrowserScreenshotRequest?(); // BrowserScreenshotRequest? |  (optional) 

            try
            {
                // Capture a page screenshot
                BrowserScreenshotPost200Response result = apiInstance.BrowserScreenshotPost(browserScreenshotRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling BrowserApi.BrowserScreenshotPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the BrowserScreenshotPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Capture a page screenshot
    ApiResponse<BrowserScreenshotPost200Response> response = apiInstance.BrowserScreenshotPostWithHttpInfo(browserScreenshotRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling BrowserApi.BrowserScreenshotPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **browserScreenshotRequest** | [**BrowserScreenshotRequest?**](BrowserScreenshotRequest?.md) |  | [optional]  |

### Return type

[**BrowserScreenshotPost200Response**](BrowserScreenshotPost200Response.md)

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

