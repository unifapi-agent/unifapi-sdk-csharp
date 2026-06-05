# Unifapi.Sdk.Api.TiktokApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**TiktokFeedRecommendedPost**](TiktokApi.md#tiktokfeedrecommendedpost) | **POST** /tiktok/feed/recommended | Get TikTok recommendation videos |
| [**TiktokHashtagsIdGet**](TiktokApi.md#tiktokhashtagsidget) | **GET** /tiktok/hashtags/{id} | Get a TikTok hashtag by ID |
| [**TiktokHashtagsIdVideosGet**](TiktokApi.md#tiktokhashtagsidvideosget) | **GET** /tiktok/hashtags/{id}/videos | List videos tagged with a TikTok hashtag |
| [**TiktokMusicIdGet**](TiktokApi.md#tiktokmusicidget) | **GET** /tiktok/music/{id} | Get a TikTok music track by ID |
| [**TiktokMusicIdVideosGet**](TiktokApi.md#tiktokmusicidvideosget) | **GET** /tiktok/music/{id}/videos | List videos using a TikTok music track |
| [**TiktokSearchGet**](TiktokApi.md#tiktoksearchget) | **GET** /tiktok/search | General TikTok search (returns videos) |
| [**TiktokSearchHashtagsGet**](TiktokApi.md#tiktoksearchhashtagsget) | **GET** /tiktok/search/hashtags | Search TikTok hashtags by keyword |
| [**TiktokSearchUsersGet**](TiktokApi.md#tiktoksearchusersget) | **GET** /tiktok/search/users | Search TikTok users by keyword |
| [**TiktokSearchVideosGet**](TiktokApi.md#tiktoksearchvideosget) | **GET** /tiktok/search/videos | Search TikTok videos by keyword |
| [**TiktokUsersIdFollowersGet**](TiktokApi.md#tiktokusersidfollowersget) | **GET** /tiktok/users/{id}/followers | List a TikTok user&#39;s followers |
| [**TiktokUsersIdFollowingGet**](TiktokApi.md#tiktokusersidfollowingget) | **GET** /tiktok/users/{id}/following | List users a TikTok user is following |
| [**TiktokUsersIdGet**](TiktokApi.md#tiktokusersidget) | **GET** /tiktok/users/{id} | Get a TikTok user profile |
| [**TiktokUsersIdLikesGet**](TiktokApi.md#tiktokusersidlikesget) | **GET** /tiktok/users/{id}/likes | List videos liked by a TikTok user |
| [**TiktokUsersIdVideosGet**](TiktokApi.md#tiktokusersidvideosget) | **GET** /tiktok/users/{id}/videos | List videos posted by a TikTok user |
| [**TiktokUsersResolveGet**](TiktokApi.md#tiktokusersresolveget) | **GET** /tiktok/users/resolve | Resolve a TikTok username to a user id |
| [**TiktokVideosBatchPost**](TiktokApi.md#tiktokvideosbatchpost) | **POST** /tiktok/videos/batch | Batch-fetch TikTok videos by ID |
| [**TiktokVideosIdCommentsCommentIdRepliesGet**](TiktokApi.md#tiktokvideosidcommentscommentidrepliesget) | **GET** /tiktok/videos/{id}/comments/{comment_id}/replies | List replies to a TikTok comment |
| [**TiktokVideosIdCommentsGet**](TiktokApi.md#tiktokvideosidcommentsget) | **GET** /tiktok/videos/{id}/comments | List top-level comments on a TikTok video |
| [**TiktokVideosIdGet**](TiktokApi.md#tiktokvideosidget) | **GET** /tiktok/videos/{id} | Get a TikTok video by ID |
| [**TiktokVideosResolveGet**](TiktokApi.md#tiktokvideosresolveget) | **GET** /tiktok/videos/resolve | Resolve a TikTok share URL to a video |

<a id="tiktokfeedrecommendedpost"></a>
# **TiktokFeedRecommendedPost**
> TiktokFeedRecommendedPost200Response TiktokFeedRecommendedPost (TiktokFeedRecommendedPostRequest? tiktokFeedRecommendedPostRequest = null)

Get TikTok recommendation videos

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokFeedRecommendedPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var tiktokFeedRecommendedPostRequest = new TiktokFeedRecommendedPostRequest?(); // TiktokFeedRecommendedPostRequest? |  (optional) 

            try
            {
                // Get TikTok recommendation videos
                TiktokFeedRecommendedPost200Response result = apiInstance.TiktokFeedRecommendedPost(tiktokFeedRecommendedPostRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokFeedRecommendedPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokFeedRecommendedPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get TikTok recommendation videos
    ApiResponse<TiktokFeedRecommendedPost200Response> response = apiInstance.TiktokFeedRecommendedPostWithHttpInfo(tiktokFeedRecommendedPostRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokFeedRecommendedPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **tiktokFeedRecommendedPostRequest** | [**TiktokFeedRecommendedPostRequest?**](TiktokFeedRecommendedPostRequest?.md) |  | [optional]  |

### Return type

[**TiktokFeedRecommendedPost200Response**](TiktokFeedRecommendedPost200Response.md)

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

<a id="tiktokhashtagsidget"></a>
# **TiktokHashtagsIdGet**
> TiktokHashtagsIdGet200Response TiktokHashtagsIdGet (string id)

Get a TikTok hashtag by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokHashtagsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | 

            try
            {
                // Get a TikTok hashtag by ID
                TiktokHashtagsIdGet200Response result = apiInstance.TiktokHashtagsIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokHashtagsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokHashtagsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a TikTok hashtag by ID
    ApiResponse<TiktokHashtagsIdGet200Response> response = apiInstance.TiktokHashtagsIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokHashtagsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**TiktokHashtagsIdGet200Response**](TiktokHashtagsIdGet200Response.md)

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

<a id="tiktokhashtagsidvideosget"></a>
# **TiktokHashtagsIdVideosGet**
> TiktokHashtagsIdVideosGet200Response TiktokHashtagsIdVideosGet (string id, string? cursor = null, int? limit = null)

List videos tagged with a TikTok hashtag

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokHashtagsIdVideosGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List videos tagged with a TikTok hashtag
                TiktokHashtagsIdVideosGet200Response result = apiInstance.TiktokHashtagsIdVideosGet(id, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokHashtagsIdVideosGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokHashtagsIdVideosGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List videos tagged with a TikTok hashtag
    ApiResponse<TiktokHashtagsIdVideosGet200Response> response = apiInstance.TiktokHashtagsIdVideosGetWithHttpInfo(id, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokHashtagsIdVideosGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokHashtagsIdVideosGet200Response**](TiktokHashtagsIdVideosGet200Response.md)

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

<a id="tiktokmusicidget"></a>
# **TiktokMusicIdGet**
> TiktokMusicIdGet200Response TiktokMusicIdGet (string id)

Get a TikTok music track by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokMusicIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | 

            try
            {
                // Get a TikTok music track by ID
                TiktokMusicIdGet200Response result = apiInstance.TiktokMusicIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokMusicIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokMusicIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a TikTok music track by ID
    ApiResponse<TiktokMusicIdGet200Response> response = apiInstance.TiktokMusicIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokMusicIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**TiktokMusicIdGet200Response**](TiktokMusicIdGet200Response.md)

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

<a id="tiktokmusicidvideosget"></a>
# **TiktokMusicIdVideosGet**
> TiktokHashtagsIdVideosGet200Response TiktokMusicIdVideosGet (string id, string? cursor = null, int? limit = null)

List videos using a TikTok music track

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokMusicIdVideosGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List videos using a TikTok music track
                TiktokHashtagsIdVideosGet200Response result = apiInstance.TiktokMusicIdVideosGet(id, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokMusicIdVideosGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokMusicIdVideosGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List videos using a TikTok music track
    ApiResponse<TiktokHashtagsIdVideosGet200Response> response = apiInstance.TiktokMusicIdVideosGetWithHttpInfo(id, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokMusicIdVideosGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokHashtagsIdVideosGet200Response**](TiktokHashtagsIdVideosGet200Response.md)

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

<a id="tiktoksearchget"></a>
# **TiktokSearchGet**
> TiktokHashtagsIdVideosGet200Response TiktokSearchGet (string q, string? cursor = null, int? limit = null)

General TikTok search (returns videos)

Returns TikTok videos for the keyword `q`. Use type-specific endpoints when needed.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokSearchGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var q = "q_example";  // string | Search keyword
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // General TikTok search (returns videos)
                TiktokHashtagsIdVideosGet200Response result = apiInstance.TiktokSearchGet(q, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokSearchGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokSearchGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // General TikTok search (returns videos)
    ApiResponse<TiktokHashtagsIdVideosGet200Response> response = apiInstance.TiktokSearchGetWithHttpInfo(q, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokSearchGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **q** | **string** | Search keyword |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokHashtagsIdVideosGet200Response**](TiktokHashtagsIdVideosGet200Response.md)

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

<a id="tiktoksearchhashtagsget"></a>
# **TiktokSearchHashtagsGet**
> TiktokSearchHashtagsGet200Response TiktokSearchHashtagsGet (string q, string? cursor = null, int? limit = null)

Search TikTok hashtags by keyword

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokSearchHashtagsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var q = "q_example";  // string | Search keyword
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // Search TikTok hashtags by keyword
                TiktokSearchHashtagsGet200Response result = apiInstance.TiktokSearchHashtagsGet(q, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokSearchHashtagsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokSearchHashtagsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search TikTok hashtags by keyword
    ApiResponse<TiktokSearchHashtagsGet200Response> response = apiInstance.TiktokSearchHashtagsGetWithHttpInfo(q, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokSearchHashtagsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **q** | **string** | Search keyword |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokSearchHashtagsGet200Response**](TiktokSearchHashtagsGet200Response.md)

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

<a id="tiktoksearchusersget"></a>
# **TiktokSearchUsersGet**
> TiktokSearchUsersGet200Response TiktokSearchUsersGet (string q, string? cursor = null, int? limit = null)

Search TikTok users by keyword

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokSearchUsersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var q = "q_example";  // string | Search keyword
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // Search TikTok users by keyword
                TiktokSearchUsersGet200Response result = apiInstance.TiktokSearchUsersGet(q, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokSearchUsersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokSearchUsersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search TikTok users by keyword
    ApiResponse<TiktokSearchUsersGet200Response> response = apiInstance.TiktokSearchUsersGetWithHttpInfo(q, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokSearchUsersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **q** | **string** | Search keyword |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokSearchUsersGet200Response**](TiktokSearchUsersGet200Response.md)

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

<a id="tiktoksearchvideosget"></a>
# **TiktokSearchVideosGet**
> TiktokHashtagsIdVideosGet200Response TiktokSearchVideosGet (string q, string? cursor = null, int? limit = null)

Search TikTok videos by keyword

Returns a paginated list of TikTok videos matching the keyword `q`. Use `next_cursor` from the response as the next request's `cursor`.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokSearchVideosGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var q = "q_example";  // string | Search keyword
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // Search TikTok videos by keyword
                TiktokHashtagsIdVideosGet200Response result = apiInstance.TiktokSearchVideosGet(q, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokSearchVideosGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokSearchVideosGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search TikTok videos by keyword
    ApiResponse<TiktokHashtagsIdVideosGet200Response> response = apiInstance.TiktokSearchVideosGetWithHttpInfo(q, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokSearchVideosGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **q** | **string** | Search keyword |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokHashtagsIdVideosGet200Response**](TiktokHashtagsIdVideosGet200Response.md)

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

<a id="tiktokusersidfollowersget"></a>
# **TiktokUsersIdFollowersGet**
> TiktokSearchUsersGet200Response TiktokUsersIdFollowersGet (string id, string? cursor = null, int? limit = null)

List a TikTok user's followers

Returns a paginated list of users following the given user.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokUsersIdFollowersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | TikTok sec_uid, numeric user id, or public handle.
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List a TikTok user's followers
                TiktokSearchUsersGet200Response result = apiInstance.TiktokUsersIdFollowersGet(id, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokUsersIdFollowersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokUsersIdFollowersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a TikTok user's followers
    ApiResponse<TiktokSearchUsersGet200Response> response = apiInstance.TiktokUsersIdFollowersGetWithHttpInfo(id, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokUsersIdFollowersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | TikTok sec_uid, numeric user id, or public handle. |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokSearchUsersGet200Response**](TiktokSearchUsersGet200Response.md)

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

<a id="tiktokusersidfollowingget"></a>
# **TiktokUsersIdFollowingGet**
> TiktokSearchUsersGet200Response TiktokUsersIdFollowingGet (string id, string? cursor = null, int? limit = null)

List users a TikTok user is following

Returns a paginated list of users the given user is following.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokUsersIdFollowingGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | TikTok sec_uid, numeric user id, or public handle.
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List users a TikTok user is following
                TiktokSearchUsersGet200Response result = apiInstance.TiktokUsersIdFollowingGet(id, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokUsersIdFollowingGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokUsersIdFollowingGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List users a TikTok user is following
    ApiResponse<TiktokSearchUsersGet200Response> response = apiInstance.TiktokUsersIdFollowingGetWithHttpInfo(id, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokUsersIdFollowingGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | TikTok sec_uid, numeric user id, or public handle. |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokSearchUsersGet200Response**](TiktokSearchUsersGet200Response.md)

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

<a id="tiktokusersidget"></a>
# **TiktokUsersIdGet**
> TiktokUsersIdGet200Response TiktokUsersIdGet (string id)

Get a TikTok user profile

Returns the canonicalized public profile for the TikTok user with the given sec_uid, numeric user id, or handle.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokUsersIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | TikTok sec_uid, numeric user id, or public handle.

            try
            {
                // Get a TikTok user profile
                TiktokUsersIdGet200Response result = apiInstance.TiktokUsersIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokUsersIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokUsersIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a TikTok user profile
    ApiResponse<TiktokUsersIdGet200Response> response = apiInstance.TiktokUsersIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokUsersIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | TikTok sec_uid, numeric user id, or public handle. |  |

### Return type

[**TiktokUsersIdGet200Response**](TiktokUsersIdGet200Response.md)

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

<a id="tiktokusersidlikesget"></a>
# **TiktokUsersIdLikesGet**
> TiktokHashtagsIdVideosGet200Response TiktokUsersIdLikesGet (string id, string? cursor = null, int? limit = null)

List videos liked by a TikTok user

Returns a paginated list of videos the user has liked where the user has made their likes public.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokUsersIdLikesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | TikTok sec_uid, numeric user id, or public handle.
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List videos liked by a TikTok user
                TiktokHashtagsIdVideosGet200Response result = apiInstance.TiktokUsersIdLikesGet(id, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokUsersIdLikesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokUsersIdLikesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List videos liked by a TikTok user
    ApiResponse<TiktokHashtagsIdVideosGet200Response> response = apiInstance.TiktokUsersIdLikesGetWithHttpInfo(id, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokUsersIdLikesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | TikTok sec_uid, numeric user id, or public handle. |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokHashtagsIdVideosGet200Response**](TiktokHashtagsIdVideosGet200Response.md)

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

<a id="tiktokusersidvideosget"></a>
# **TiktokUsersIdVideosGet**
> TiktokHashtagsIdVideosGet200Response TiktokUsersIdVideosGet (string id, string? cursor = null, int? limit = null)

List videos posted by a TikTok user

Returns a paginated list of public videos posted by the user. Use `next_cursor` from the response as the next request's `cursor`.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokUsersIdVideosGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | TikTok sec_uid, numeric user id, or public handle.
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List videos posted by a TikTok user
                TiktokHashtagsIdVideosGet200Response result = apiInstance.TiktokUsersIdVideosGet(id, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokUsersIdVideosGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokUsersIdVideosGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List videos posted by a TikTok user
    ApiResponse<TiktokHashtagsIdVideosGet200Response> response = apiInstance.TiktokUsersIdVideosGetWithHttpInfo(id, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokUsersIdVideosGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | TikTok sec_uid, numeric user id, or public handle. |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokHashtagsIdVideosGet200Response**](TiktokHashtagsIdVideosGet200Response.md)

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

<a id="tiktokusersresolveget"></a>
# **TiktokUsersResolveGet**
> TiktokUsersResolveGet200Response TiktokUsersResolveGet (string username)

Resolve a TikTok username to a user id

Accepts a public TikTok username (handle) and returns the user's stable opaque id for other /tiktok/users/{id} endpoints.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokUsersResolveGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var username = "username_example";  // string | Public TikTok handle, e.g. 'jennmelon'

            try
            {
                // Resolve a TikTok username to a user id
                TiktokUsersResolveGet200Response result = apiInstance.TiktokUsersResolveGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokUsersResolveGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokUsersResolveGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Resolve a TikTok username to a user id
    ApiResponse<TiktokUsersResolveGet200Response> response = apiInstance.TiktokUsersResolveGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokUsersResolveGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** | Public TikTok handle, e.g. &#39;jennmelon&#39; |  |

### Return type

[**TiktokUsersResolveGet200Response**](TiktokUsersResolveGet200Response.md)

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

<a id="tiktokvideosbatchpost"></a>
# **TiktokVideosBatchPost**
> TiktokFeedRecommendedPost200Response TiktokVideosBatchPost (TiktokVideosBatchPostRequest? tiktokVideosBatchPostRequest = null)

Batch-fetch TikTok videos by ID

Returns canonicalized metadata for up to 20 TikTok videos.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokVideosBatchPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var tiktokVideosBatchPostRequest = new TiktokVideosBatchPostRequest?(); // TiktokVideosBatchPostRequest? |  (optional) 

            try
            {
                // Batch-fetch TikTok videos by ID
                TiktokFeedRecommendedPost200Response result = apiInstance.TiktokVideosBatchPost(tiktokVideosBatchPostRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokVideosBatchPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokVideosBatchPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Batch-fetch TikTok videos by ID
    ApiResponse<TiktokFeedRecommendedPost200Response> response = apiInstance.TiktokVideosBatchPostWithHttpInfo(tiktokVideosBatchPostRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokVideosBatchPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **tiktokVideosBatchPostRequest** | [**TiktokVideosBatchPostRequest?**](TiktokVideosBatchPostRequest?.md) |  | [optional]  |

### Return type

[**TiktokFeedRecommendedPost200Response**](TiktokFeedRecommendedPost200Response.md)

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

<a id="tiktokvideosidcommentscommentidrepliesget"></a>
# **TiktokVideosIdCommentsCommentIdRepliesGet**
> TiktokVideosIdCommentsCommentIdRepliesGet200Response TiktokVideosIdCommentsCommentIdRepliesGet (string id, string commentId, string? cursor = null, int? limit = null)

List replies to a TikTok comment

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokVideosIdCommentsCommentIdRepliesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | 
            var commentId = "commentId_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List replies to a TikTok comment
                TiktokVideosIdCommentsCommentIdRepliesGet200Response result = apiInstance.TiktokVideosIdCommentsCommentIdRepliesGet(id, commentId, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokVideosIdCommentsCommentIdRepliesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokVideosIdCommentsCommentIdRepliesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List replies to a TikTok comment
    ApiResponse<TiktokVideosIdCommentsCommentIdRepliesGet200Response> response = apiInstance.TiktokVideosIdCommentsCommentIdRepliesGetWithHttpInfo(id, commentId, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokVideosIdCommentsCommentIdRepliesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **commentId** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokVideosIdCommentsCommentIdRepliesGet200Response**](TiktokVideosIdCommentsCommentIdRepliesGet200Response.md)

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

<a id="tiktokvideosidcommentsget"></a>
# **TiktokVideosIdCommentsGet**
> TiktokVideosIdCommentsCommentIdRepliesGet200Response TiktokVideosIdCommentsGet (string id, string? cursor = null, int? limit = null)

List top-level comments on a TikTok video

Returns a paginated list of top-level comments on the given video. Use `next_cursor` from the response as the next request's `cursor`.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokVideosIdCommentsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var limit = 20;  // int? |  (optional)  (default to 20)

            try
            {
                // List top-level comments on a TikTok video
                TiktokVideosIdCommentsCommentIdRepliesGet200Response result = apiInstance.TiktokVideosIdCommentsGet(id, cursor, limit);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokVideosIdCommentsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokVideosIdCommentsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List top-level comments on a TikTok video
    ApiResponse<TiktokVideosIdCommentsCommentIdRepliesGet200Response> response = apiInstance.TiktokVideosIdCommentsGetWithHttpInfo(id, cursor, limit);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokVideosIdCommentsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **limit** | **int?** |  | [optional] [default to 20] |

### Return type

[**TiktokVideosIdCommentsCommentIdRepliesGet200Response**](TiktokVideosIdCommentsCommentIdRepliesGet200Response.md)

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

<a id="tiktokvideosidget"></a>
# **TiktokVideosIdGet**
> TiktokVideosIdGet200Response TiktokVideosIdGet (string id)

Get a TikTok video by ID

Returns canonicalized metadata for a single TikTok video. The `{id}` must be the numeric TikTok video id.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokVideosIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var id = "id_example";  // string | 

            try
            {
                // Get a TikTok video by ID
                TiktokVideosIdGet200Response result = apiInstance.TiktokVideosIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokVideosIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokVideosIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a TikTok video by ID
    ApiResponse<TiktokVideosIdGet200Response> response = apiInstance.TiktokVideosIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokVideosIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**TiktokVideosIdGet200Response**](TiktokVideosIdGet200Response.md)

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

<a id="tiktokvideosresolveget"></a>
# **TiktokVideosResolveGet**
> TiktokVideosIdGet200Response TiktokVideosResolveGet (string url)

Resolve a TikTok share URL to a video

Accepts a TikTok share URL (long or short / vm.tiktok.com) and returns the canonical Video object.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class TiktokVideosResolveGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new TiktokApi(config);
            var url = "url_example";  // string | TikTok share URL (long or short form)

            try
            {
                // Resolve a TikTok share URL to a video
                TiktokVideosIdGet200Response result = apiInstance.TiktokVideosResolveGet(url);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling TiktokApi.TiktokVideosResolveGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the TiktokVideosResolveGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Resolve a TikTok share URL to a video
    ApiResponse<TiktokVideosIdGet200Response> response = apiInstance.TiktokVideosResolveGetWithHttpInfo(url);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling TiktokApi.TiktokVideosResolveGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **url** | **string** | TikTok share URL (long or short form) |  |

### Return type

[**TiktokVideosIdGet200Response**](TiktokVideosIdGet200Response.md)

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

