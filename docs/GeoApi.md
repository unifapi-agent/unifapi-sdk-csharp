# Unifapi.Sdk.Api.GeoApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GeoKeywordsSearchVolumePost**](GeoApi.md#geokeywordssearchvolumepost) | **POST** /geo/keywords/search-volume | Get AI search volume for keywords |
| [**GeoMentionsAggregatedMetricsPost**](GeoApi.md#geomentionsaggregatedmetricspost) | **POST** /geo/mentions/aggregated-metrics | Aggregate LLM mention metrics by dimension |
| [**GeoMentionsCrossAggregatedMetricsPost**](GeoApi.md#geomentionscrossaggregatedmetricspost) | **POST** /geo/mentions/cross-aggregated-metrics | Compare LLM mentions across labeled groups |
| [**GeoMentionsSearchPost**](GeoApi.md#geomentionssearchpost) | **POST** /geo/mentions/search | Search LLM mentions of a domain or keyword |
| [**GeoMentionsTopDomainsPost**](GeoApi.md#geomentionstopdomainspost) | **POST** /geo/mentions/top-domains | List domains most cited in LLM answers |
| [**GeoMentionsTopPagesPost**](GeoApi.md#geomentionstoppagespost) | **POST** /geo/mentions/top-pages | List pages most cited in LLM answers |
| [**GeoSerpPost**](GeoApi.md#geoserppost) | **POST** /geo/serp | Search AI Mode generative results |

<a id="geokeywordssearchvolumepost"></a>
# **GeoKeywordsSearchVolumePost**
> GeoKeywordsSearchVolumePost200Response GeoKeywordsSearchVolumePost (GeoKeywordSearchVolumeRequest? geoKeywordSearchVolumeRequest = null)

Get AI search volume for keywords

Look up generative-AI search volume and monthly trend for up to 1000 keywords in a location and language.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class GeoKeywordsSearchVolumePostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new GeoApi(config);
            var geoKeywordSearchVolumeRequest = new GeoKeywordSearchVolumeRequest?(); // GeoKeywordSearchVolumeRequest? |  (optional) 

            try
            {
                // Get AI search volume for keywords
                GeoKeywordsSearchVolumePost200Response result = apiInstance.GeoKeywordsSearchVolumePost(geoKeywordSearchVolumeRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GeoApi.GeoKeywordsSearchVolumePost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GeoKeywordsSearchVolumePostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get AI search volume for keywords
    ApiResponse<GeoKeywordsSearchVolumePost200Response> response = apiInstance.GeoKeywordsSearchVolumePostWithHttpInfo(geoKeywordSearchVolumeRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GeoApi.GeoKeywordsSearchVolumePostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **geoKeywordSearchVolumeRequest** | [**GeoKeywordSearchVolumeRequest?**](GeoKeywordSearchVolumeRequest?.md) |  | [optional]  |

### Return type

[**GeoKeywordsSearchVolumePost200Response**](GeoKeywordsSearchVolumePost200Response.md)

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

<a id="geomentionsaggregatedmetricspost"></a>
# **GeoMentionsAggregatedMetricsPost**
> GeoMentionsAggregatedMetricsPost200Response GeoMentionsAggregatedMetricsPost (GeoMentionsAggregatedMetricsRequest? geoMentionsAggregatedMetricsRequest = null)

Aggregate LLM mention metrics by dimension

Aggregate LLM mentions of a domain or keyword across platform, location, language, source/search-result domains, and brand entities.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class GeoMentionsAggregatedMetricsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new GeoApi(config);
            var geoMentionsAggregatedMetricsRequest = new GeoMentionsAggregatedMetricsRequest?(); // GeoMentionsAggregatedMetricsRequest? |  (optional) 

            try
            {
                // Aggregate LLM mention metrics by dimension
                GeoMentionsAggregatedMetricsPost200Response result = apiInstance.GeoMentionsAggregatedMetricsPost(geoMentionsAggregatedMetricsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GeoApi.GeoMentionsAggregatedMetricsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GeoMentionsAggregatedMetricsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Aggregate LLM mention metrics by dimension
    ApiResponse<GeoMentionsAggregatedMetricsPost200Response> response = apiInstance.GeoMentionsAggregatedMetricsPostWithHttpInfo(geoMentionsAggregatedMetricsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GeoApi.GeoMentionsAggregatedMetricsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **geoMentionsAggregatedMetricsRequest** | [**GeoMentionsAggregatedMetricsRequest?**](GeoMentionsAggregatedMetricsRequest?.md) |  | [optional]  |

### Return type

[**GeoMentionsAggregatedMetricsPost200Response**](GeoMentionsAggregatedMetricsPost200Response.md)

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

<a id="geomentionscrossaggregatedmetricspost"></a>
# **GeoMentionsCrossAggregatedMetricsPost**
> GeoMentionsCrossAggregatedMetricsPost200Response GeoMentionsCrossAggregatedMetricsPost (GeoMentionsCrossAggregatedMetricsRequest? geoMentionsCrossAggregatedMetricsRequest = null)

Compare LLM mentions across labeled groups

Aggregate and compare LLM mention metrics across several labeled target groups for side-by-side share-of-voice analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class GeoMentionsCrossAggregatedMetricsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new GeoApi(config);
            var geoMentionsCrossAggregatedMetricsRequest = new GeoMentionsCrossAggregatedMetricsRequest?(); // GeoMentionsCrossAggregatedMetricsRequest? |  (optional) 

            try
            {
                // Compare LLM mentions across labeled groups
                GeoMentionsCrossAggregatedMetricsPost200Response result = apiInstance.GeoMentionsCrossAggregatedMetricsPost(geoMentionsCrossAggregatedMetricsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GeoApi.GeoMentionsCrossAggregatedMetricsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GeoMentionsCrossAggregatedMetricsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Compare LLM mentions across labeled groups
    ApiResponse<GeoMentionsCrossAggregatedMetricsPost200Response> response = apiInstance.GeoMentionsCrossAggregatedMetricsPostWithHttpInfo(geoMentionsCrossAggregatedMetricsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GeoApi.GeoMentionsCrossAggregatedMetricsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **geoMentionsCrossAggregatedMetricsRequest** | [**GeoMentionsCrossAggregatedMetricsRequest?**](GeoMentionsCrossAggregatedMetricsRequest?.md) |  | [optional]  |

### Return type

[**GeoMentionsCrossAggregatedMetricsPost200Response**](GeoMentionsCrossAggregatedMetricsPost200Response.md)

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

<a id="geomentionssearchpost"></a>
# **GeoMentionsSearchPost**
> GeoMentionsSearchPost200Response GeoMentionsSearchPost (GeoMentionsSearchRequest? geoMentionsSearchRequest = null)

Search LLM mentions of a domain or keyword

Find where a domain or keyword is mentioned across ChatGPT and AI search answers, with the question, answer, cited sources, and AI search volume.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class GeoMentionsSearchPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new GeoApi(config);
            var geoMentionsSearchRequest = new GeoMentionsSearchRequest?(); // GeoMentionsSearchRequest? |  (optional) 

            try
            {
                // Search LLM mentions of a domain or keyword
                GeoMentionsSearchPost200Response result = apiInstance.GeoMentionsSearchPost(geoMentionsSearchRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GeoApi.GeoMentionsSearchPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GeoMentionsSearchPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search LLM mentions of a domain or keyword
    ApiResponse<GeoMentionsSearchPost200Response> response = apiInstance.GeoMentionsSearchPostWithHttpInfo(geoMentionsSearchRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GeoApi.GeoMentionsSearchPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **geoMentionsSearchRequest** | [**GeoMentionsSearchRequest?**](GeoMentionsSearchRequest?.md) |  | [optional]  |

### Return type

[**GeoMentionsSearchPost200Response**](GeoMentionsSearchPost200Response.md)

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

<a id="geomentionstopdomainspost"></a>
# **GeoMentionsTopDomainsPost**
> GeoMentionsTopDomainsPost200Response GeoMentionsTopDomainsPost (GeoMentionsTopDomainsRequest? geoMentionsTopDomainsRequest = null)

List domains most cited in LLM answers

Rank the domains most frequently cited as sources in LLM answers for a target domain or keyword, with per-dimension breakdowns.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class GeoMentionsTopDomainsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new GeoApi(config);
            var geoMentionsTopDomainsRequest = new GeoMentionsTopDomainsRequest?(); // GeoMentionsTopDomainsRequest? |  (optional) 

            try
            {
                // List domains most cited in LLM answers
                GeoMentionsTopDomainsPost200Response result = apiInstance.GeoMentionsTopDomainsPost(geoMentionsTopDomainsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GeoApi.GeoMentionsTopDomainsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GeoMentionsTopDomainsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List domains most cited in LLM answers
    ApiResponse<GeoMentionsTopDomainsPost200Response> response = apiInstance.GeoMentionsTopDomainsPostWithHttpInfo(geoMentionsTopDomainsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GeoApi.GeoMentionsTopDomainsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **geoMentionsTopDomainsRequest** | [**GeoMentionsTopDomainsRequest?**](GeoMentionsTopDomainsRequest?.md) |  | [optional]  |

### Return type

[**GeoMentionsTopDomainsPost200Response**](GeoMentionsTopDomainsPost200Response.md)

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

<a id="geomentionstoppagespost"></a>
# **GeoMentionsTopPagesPost**
> GeoMentionsTopPagesPost200Response GeoMentionsTopPagesPost (GeoMentionsTopPagesRequest? geoMentionsTopPagesRequest = null)

List pages most cited in LLM answers

Rank the pages most frequently cited as sources in LLM answers for a target domain or keyword, with per-dimension breakdowns.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class GeoMentionsTopPagesPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new GeoApi(config);
            var geoMentionsTopPagesRequest = new GeoMentionsTopPagesRequest?(); // GeoMentionsTopPagesRequest? |  (optional) 

            try
            {
                // List pages most cited in LLM answers
                GeoMentionsTopPagesPost200Response result = apiInstance.GeoMentionsTopPagesPost(geoMentionsTopPagesRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GeoApi.GeoMentionsTopPagesPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GeoMentionsTopPagesPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List pages most cited in LLM answers
    ApiResponse<GeoMentionsTopPagesPost200Response> response = apiInstance.GeoMentionsTopPagesPostWithHttpInfo(geoMentionsTopPagesRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GeoApi.GeoMentionsTopPagesPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **geoMentionsTopPagesRequest** | [**GeoMentionsTopPagesRequest?**](GeoMentionsTopPagesRequest?.md) |  | [optional]  |

### Return type

[**GeoMentionsTopPagesPost200Response**](GeoMentionsTopPagesPost200Response.md)

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

<a id="geoserppost"></a>
# **GeoSerpPost**
> GeoSerpPost200Response GeoSerpPost (GeoSerpRequest? geoSerpRequest = null)

Search AI Mode generative results

Run one live AI Mode search for generative answer evidence, cited sources, and target-domain visibility.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class GeoSerpPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new GeoApi(config);
            var geoSerpRequest = new GeoSerpRequest?(); // GeoSerpRequest? |  (optional) 

            try
            {
                // Search AI Mode generative results
                GeoSerpPost200Response result = apiInstance.GeoSerpPost(geoSerpRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling GeoApi.GeoSerpPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the GeoSerpPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search AI Mode generative results
    ApiResponse<GeoSerpPost200Response> response = apiInstance.GeoSerpPostWithHttpInfo(geoSerpRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling GeoApi.GeoSerpPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **geoSerpRequest** | [**GeoSerpRequest?**](GeoSerpRequest?.md) |  | [optional]  |

### Return type

[**GeoSerpPost200Response**](GeoSerpPost200Response.md)

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

