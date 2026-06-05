# Unifapi.Sdk.Api.HackerNewsApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**HackerNewsItemsIdGet**](HackerNewsApi.md#hackernewsitemsidget) | **GET** /hacker-news/items/{id} | Get Hacker News item by ID |
| [**HackerNewsMaxItemGet**](HackerNewsApi.md#hackernewsmaxitemget) | **GET** /hacker-news/max-item | Get largest Hacker News item ID |
| [**HackerNewsStoriesFeedGet**](HackerNewsApi.md#hackernewsstoriesfeedget) | **GET** /hacker-news/stories/{feed} | List Hacker News story IDs |
| [**HackerNewsStoriesFeedItemsGet**](HackerNewsApi.md#hackernewsstoriesfeeditemsget) | **GET** /hacker-news/stories/{feed}/items | List Hacker News story items |
| [**HackerNewsUpdatesGet**](HackerNewsApi.md#hackernewsupdatesget) | **GET** /hacker-news/updates | Get changed Hacker News items and profiles |
| [**HackerNewsUsersIdGet**](HackerNewsApi.md#hackernewsusersidget) | **GET** /hacker-news/users/{id} | Get Hacker News user by ID |

<a id="hackernewsitemsidget"></a>
# **HackerNewsItemsIdGet**
> HackerNewsItemsIdGet200Response HackerNewsItemsIdGet (int id)

Get Hacker News item by ID

Fetch a single Hacker News item. Stories, comments, jobs, polls, and poll options share the same item shape.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HackerNewsItemsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HackerNewsApi(config);
            var id = 56;  // int | Hacker News item id.

            try
            {
                // Get Hacker News item by ID
                HackerNewsItemsIdGet200Response result = apiInstance.HackerNewsItemsIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HackerNewsApi.HackerNewsItemsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HackerNewsItemsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get Hacker News item by ID
    ApiResponse<HackerNewsItemsIdGet200Response> response = apiInstance.HackerNewsItemsIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HackerNewsApi.HackerNewsItemsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **int** | Hacker News item id. |  |

### Return type

[**HackerNewsItemsIdGet200Response**](HackerNewsItemsIdGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
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

<a id="hackernewsmaxitemget"></a>
# **HackerNewsMaxItemGet**
> HackerNewsMaxItemGet200Response HackerNewsMaxItemGet ()

Get largest Hacker News item ID

Returns the current largest Hacker News item id.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HackerNewsMaxItemGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HackerNewsApi(config);

            try
            {
                // Get largest Hacker News item ID
                HackerNewsMaxItemGet200Response result = apiInstance.HackerNewsMaxItemGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HackerNewsApi.HackerNewsMaxItemGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HackerNewsMaxItemGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get largest Hacker News item ID
    ApiResponse<HackerNewsMaxItemGet200Response> response = apiInstance.HackerNewsMaxItemGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HackerNewsApi.HackerNewsMaxItemGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**HackerNewsMaxItemGet200Response**](HackerNewsMaxItemGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
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

<a id="hackernewsstoriesfeedget"></a>
# **HackerNewsStoriesFeedGet**
> HackerNewsStoriesFeedGet200Response HackerNewsStoriesFeedGet (HackerNewsStoryFeed feed, string? cursor = null, int? limit = null)

List Hacker News story IDs

List Hacker News story ids from a named feed. Use `/hacker-news/items/{id}` to fetch item details.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HackerNewsStoriesFeedGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HackerNewsApi(config);
            var feed = (HackerNewsStoryFeed) "top";  // HackerNewsStoryFeed | Story feed: top, new, best, ask, show, or jobs.
            var cursor = "cursor_example";  // string? | Zero-based offset cursor returned as `next_cursor`. (optional) 
            var limit = 100;  // int? |  (optional)  (default to 100)

            try
            {
                // List Hacker News story IDs
                HackerNewsStoriesFeedGet200Response result = apiInstance.HackerNewsStoriesFeedGet(feed, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HackerNewsApi.HackerNewsStoriesFeedGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HackerNewsStoriesFeedGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Hacker News story IDs
    ApiResponse<HackerNewsStoriesFeedGet200Response> response = apiInstance.HackerNewsStoriesFeedGetWithHttpInfo(feed, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HackerNewsApi.HackerNewsStoriesFeedGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **feed** | **HackerNewsStoryFeed** | Story feed: top, new, best, ask, show, or jobs. |  |
| **cursor** | **string?** | Zero-based offset cursor returned as &#x60;next_cursor&#x60;. | [optional]  |
| **limit** | **int?** |  | [optional] [default to 100] |

### Return type

[**HackerNewsStoriesFeedGet200Response**](HackerNewsStoriesFeedGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
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

<a id="hackernewsstoriesfeeditemsget"></a>
# **HackerNewsStoriesFeedItemsGet**
> HackerNewsStoriesFeedItemsGet200Response HackerNewsStoriesFeedItemsGet (HackerNewsStoryFeed feed, string? cursor = null, int? limit = null)

List Hacker News story items

Fetch item details from a named Hacker News story feed in one operation. Use this when an agent needs readable story titles, URLs, scores, authors, or comment counts.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HackerNewsStoriesFeedItemsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HackerNewsApi(config);
            var feed = (HackerNewsStoryFeed) "top";  // HackerNewsStoryFeed | Story feed: top, new, best, ask, show, or jobs.
            var cursor = "cursor_example";  // string? | Zero-based offset cursor returned as `next_cursor`. (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List Hacker News story items
                HackerNewsStoriesFeedItemsGet200Response result = apiInstance.HackerNewsStoriesFeedItemsGet(feed, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HackerNewsApi.HackerNewsStoriesFeedItemsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HackerNewsStoriesFeedItemsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Hacker News story items
    ApiResponse<HackerNewsStoriesFeedItemsGet200Response> response = apiInstance.HackerNewsStoriesFeedItemsGetWithHttpInfo(feed, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HackerNewsApi.HackerNewsStoriesFeedItemsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **feed** | **HackerNewsStoryFeed** | Story feed: top, new, best, ask, show, or jobs. |  |
| **cursor** | **string?** | Zero-based offset cursor returned as &#x60;next_cursor&#x60;. | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**HackerNewsStoriesFeedItemsGet200Response**](HackerNewsStoriesFeedItemsGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
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

<a id="hackernewsupdatesget"></a>
# **HackerNewsUpdatesGet**
> HackerNewsUpdatesGet200Response HackerNewsUpdatesGet ()

Get changed Hacker News items and profiles

Returns recently changed Hacker News item ids and user profile ids.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HackerNewsUpdatesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HackerNewsApi(config);

            try
            {
                // Get changed Hacker News items and profiles
                HackerNewsUpdatesGet200Response result = apiInstance.HackerNewsUpdatesGet();
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HackerNewsApi.HackerNewsUpdatesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HackerNewsUpdatesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get changed Hacker News items and profiles
    ApiResponse<HackerNewsUpdatesGet200Response> response = apiInstance.HackerNewsUpdatesGetWithHttpInfo();
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HackerNewsApi.HackerNewsUpdatesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
### Return type

[**HackerNewsUpdatesGet200Response**](HackerNewsUpdatesGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
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

<a id="hackernewsusersidget"></a>
# **HackerNewsUsersIdGet**
> HackerNewsUsersIdGet200Response HackerNewsUsersIdGet (string id)

Get Hacker News user by ID

Fetch a public Hacker News user profile by case-sensitive username.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class HackerNewsUsersIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new HackerNewsApi(config);
            var id = "id_example";  // string | Case-sensitive Hacker News username.

            try
            {
                // Get Hacker News user by ID
                HackerNewsUsersIdGet200Response result = apiInstance.HackerNewsUsersIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling HackerNewsApi.HackerNewsUsersIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the HackerNewsUsersIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get Hacker News user by ID
    ApiResponse<HackerNewsUsersIdGet200Response> response = apiInstance.HackerNewsUsersIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling HackerNewsApi.HackerNewsUsersIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | Case-sensitive Hacker News username. |  |

### Return type

[**HackerNewsUsersIdGet200Response**](HackerNewsUsersIdGet200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
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

