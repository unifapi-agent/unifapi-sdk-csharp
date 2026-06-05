# Unifapi.Sdk.Api.YoutubeApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**YoutubeChannelsChannelIdGet**](YoutubeApi.md#youtubechannelschannelidget) | **GET** /youtube/channels/{channel_id} | Get a YouTube channel by id |
| [**YoutubeChannelsChannelIdShortsGet**](YoutubeApi.md#youtubechannelschannelidshortsget) | **GET** /youtube/channels/{channel_id}/shorts | List Shorts uploaded by a YouTube channel |
| [**YoutubeChannelsChannelIdVideosGet**](YoutubeApi.md#youtubechannelschannelidvideosget) | **GET** /youtube/channels/{channel_id}/videos | List videos uploaded by a YouTube channel |
| [**YoutubeResolveChannelIdGet**](YoutubeApi.md#youtuberesolvechannelidget) | **GET** /youtube/resolve/channel-id | Resolve a YouTube channel URL to its UC… channel id |
| [**YoutubeSearchGet**](YoutubeApi.md#youtubesearchget) | **GET** /youtube/search | Search YouTube videos by keyword |
| [**YoutubeTrendingGet**](YoutubeApi.md#youtubetrendingget) | **GET** /youtube/trending | Browse YouTube&#39;s trending videos |
| [**YoutubeVideosVideoIdGet**](YoutubeApi.md#youtubevideosvideoidget) | **GET** /youtube/videos/{video_id} | Get a YouTube video by id |
| [**YoutubeVideosVideoIdRelatedGet**](YoutubeApi.md#youtubevideosvideoidrelatedget) | **GET** /youtube/videos/{video_id}/related | List YouTube videos related to a given video |

<a id="youtubechannelschannelidget"></a>
# **YoutubeChannelsChannelIdGet**
> YoutubeChannelsChannelIdGet200Response YoutubeChannelsChannelIdGet (string channelId)

Get a YouTube channel by id

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeChannelsChannelIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var channelId = "channelId_example";  // string | YouTube channel id (`UCxxx...`).

            try
            {
                // Get a YouTube channel by id
                YoutubeChannelsChannelIdGet200Response result = apiInstance.YoutubeChannelsChannelIdGet(channelId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeChannelsChannelIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeChannelsChannelIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a YouTube channel by id
    ApiResponse<YoutubeChannelsChannelIdGet200Response> response = apiInstance.YoutubeChannelsChannelIdGetWithHttpInfo(channelId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeChannelsChannelIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **channelId** | **string** | YouTube channel id (&#x60;UCxxx...&#x60;). |  |

### Return type

[**YoutubeChannelsChannelIdGet200Response**](YoutubeChannelsChannelIdGet200Response.md)

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

<a id="youtubechannelschannelidshortsget"></a>
# **YoutubeChannelsChannelIdShortsGet**
> YoutubeChannelsChannelIdShortsGet200Response YoutubeChannelsChannelIdShortsGet (string channelId, string? cursor = null)

List Shorts uploaded by a YouTube channel

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeChannelsChannelIdShortsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var channelId = "channelId_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List Shorts uploaded by a YouTube channel
                YoutubeChannelsChannelIdShortsGet200Response result = apiInstance.YoutubeChannelsChannelIdShortsGet(channelId, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeChannelsChannelIdShortsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeChannelsChannelIdShortsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Shorts uploaded by a YouTube channel
    ApiResponse<YoutubeChannelsChannelIdShortsGet200Response> response = apiInstance.YoutubeChannelsChannelIdShortsGetWithHttpInfo(channelId, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeChannelsChannelIdShortsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **channelId** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**YoutubeChannelsChannelIdShortsGet200Response**](YoutubeChannelsChannelIdShortsGet200Response.md)

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

<a id="youtubechannelschannelidvideosget"></a>
# **YoutubeChannelsChannelIdVideosGet**
> YoutubeChannelsChannelIdShortsGet200Response YoutubeChannelsChannelIdVideosGet (string channelId, string? cursor = null)

List videos uploaded by a YouTube channel

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeChannelsChannelIdVideosGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var channelId = "channelId_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List videos uploaded by a YouTube channel
                YoutubeChannelsChannelIdShortsGet200Response result = apiInstance.YoutubeChannelsChannelIdVideosGet(channelId, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeChannelsChannelIdVideosGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeChannelsChannelIdVideosGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List videos uploaded by a YouTube channel
    ApiResponse<YoutubeChannelsChannelIdShortsGet200Response> response = apiInstance.YoutubeChannelsChannelIdVideosGetWithHttpInfo(channelId, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeChannelsChannelIdVideosGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **channelId** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**YoutubeChannelsChannelIdShortsGet200Response**](YoutubeChannelsChannelIdShortsGet200Response.md)

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

<a id="youtuberesolvechannelidget"></a>
# **YoutubeResolveChannelIdGet**
> YoutubeResolveChannelIdGet200Response YoutubeResolveChannelIdGet (string url)

Resolve a YouTube channel URL to its UC… channel id

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeResolveChannelIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var url = "url_example";  // string | Full channel URL — supports `youtube.com/@handle`, `/channel/UC…`, `/c/name`.

            try
            {
                // Resolve a YouTube channel URL to its UC… channel id
                YoutubeResolveChannelIdGet200Response result = apiInstance.YoutubeResolveChannelIdGet(url);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeResolveChannelIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeResolveChannelIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Resolve a YouTube channel URL to its UC… channel id
    ApiResponse<YoutubeResolveChannelIdGet200Response> response = apiInstance.YoutubeResolveChannelIdGetWithHttpInfo(url);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeResolveChannelIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **url** | **string** | Full channel URL — supports &#x60;youtube.com/@handle&#x60;, &#x60;/channel/UC…&#x60;, &#x60;/c/name&#x60;. |  |

### Return type

[**YoutubeResolveChannelIdGet200Response**](YoutubeResolveChannelIdGet200Response.md)

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

<a id="youtubesearchget"></a>
# **YoutubeSearchGet**
> YoutubeChannelsChannelIdShortsGet200Response YoutubeSearchGet (string q, string? cursor = null)

Search YouTube videos by keyword

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeSearchGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var q = "q_example";  // string | Search keyword.
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // Search YouTube videos by keyword
                YoutubeChannelsChannelIdShortsGet200Response result = apiInstance.YoutubeSearchGet(q, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeSearchGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeSearchGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search YouTube videos by keyword
    ApiResponse<YoutubeChannelsChannelIdShortsGet200Response> response = apiInstance.YoutubeSearchGetWithHttpInfo(q, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeSearchGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **q** | **string** | Search keyword. |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**YoutubeChannelsChannelIdShortsGet200Response**](YoutubeChannelsChannelIdShortsGet200Response.md)

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

<a id="youtubetrendingget"></a>
# **YoutubeTrendingGet**
> YoutubeTrendingGet200Response YoutubeTrendingGet (string? languageCode = null)

Browse YouTube's trending videos

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeTrendingGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var languageCode = "languageCode_example";  // string? | Optional language code, e.g. `en`. (optional) 

            try
            {
                // Browse YouTube's trending videos
                YoutubeTrendingGet200Response result = apiInstance.YoutubeTrendingGet(languageCode);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeTrendingGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeTrendingGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Browse YouTube's trending videos
    ApiResponse<YoutubeTrendingGet200Response> response = apiInstance.YoutubeTrendingGetWithHttpInfo(languageCode);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeTrendingGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **languageCode** | **string?** | Optional language code, e.g. &#x60;en&#x60;. | [optional]  |

### Return type

[**YoutubeTrendingGet200Response**](YoutubeTrendingGet200Response.md)

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

<a id="youtubevideosvideoidget"></a>
# **YoutubeVideosVideoIdGet**
> YoutubeVideosVideoIdGet200Response YoutubeVideosVideoIdGet (string videoId)

Get a YouTube video by id

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeVideosVideoIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var videoId = "videoId_example";  // string | YouTube video id, e.g. `oaSNBz4qMQY`.

            try
            {
                // Get a YouTube video by id
                YoutubeVideosVideoIdGet200Response result = apiInstance.YoutubeVideosVideoIdGet(videoId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeVideosVideoIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeVideosVideoIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a YouTube video by id
    ApiResponse<YoutubeVideosVideoIdGet200Response> response = apiInstance.YoutubeVideosVideoIdGetWithHttpInfo(videoId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeVideosVideoIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **videoId** | **string** | YouTube video id, e.g. &#x60;oaSNBz4qMQY&#x60;. |  |

### Return type

[**YoutubeVideosVideoIdGet200Response**](YoutubeVideosVideoIdGet200Response.md)

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

<a id="youtubevideosvideoidrelatedget"></a>
# **YoutubeVideosVideoIdRelatedGet**
> YoutubeChannelsChannelIdShortsGet200Response YoutubeVideosVideoIdRelatedGet (string videoId, string? cursor = null)

List YouTube videos related to a given video

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class YoutubeVideosVideoIdRelatedGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new YoutubeApi(config);
            var videoId = "videoId_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List YouTube videos related to a given video
                YoutubeChannelsChannelIdShortsGet200Response result = apiInstance.YoutubeVideosVideoIdRelatedGet(videoId, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling YoutubeApi.YoutubeVideosVideoIdRelatedGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the YoutubeVideosVideoIdRelatedGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List YouTube videos related to a given video
    ApiResponse<YoutubeChannelsChannelIdShortsGet200Response> response = apiInstance.YoutubeVideosVideoIdRelatedGetWithHttpInfo(videoId, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling YoutubeApi.YoutubeVideosVideoIdRelatedGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **videoId** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**YoutubeChannelsChannelIdShortsGet200Response**](YoutubeChannelsChannelIdShortsGet200Response.md)

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

