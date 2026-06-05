# Unifapi.Sdk.Api.InstagramApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**InstagramExploreGet**](InstagramApi.md#instagramexploreget) | **GET** /instagram/explore | Browse Instagram&#39;s Explore feed |
| [**InstagramLocationsIdGet**](InstagramApi.md#instagramlocationsidget) | **GET** /instagram/locations/{id} | Get an Instagram location by id |
| [**InstagramLocationsIdNearbyGet**](InstagramApi.md#instagramlocationsidnearbyget) | **GET** /instagram/locations/{id}/nearby | List Instagram locations geographically near a given location |
| [**InstagramLocationsIdPostsGet**](InstagramApi.md#instagramlocationsidpostsget) | **GET** /instagram/locations/{id}/posts | List posts tagged with an Instagram location |
| [**InstagramPostsShortcodeCommentsCommentIdRepliesGet**](InstagramApi.md#instagrampostsshortcodecommentscommentidrepliesget) | **GET** /instagram/posts/{shortcode}/comments/{commentId}/replies | List replies to an Instagram comment |
| [**InstagramPostsShortcodeCommentsGet**](InstagramApi.md#instagrampostsshortcodecommentsget) | **GET** /instagram/posts/{shortcode}/comments | List comments on an Instagram post |
| [**InstagramPostsShortcodeGet**](InstagramApi.md#instagrampostsshortcodeget) | **GET** /instagram/posts/{shortcode} | Get an Instagram post (photo / video / carousel / reel) by shortcode |
| [**InstagramReelsRecommendedGet**](InstagramApi.md#instagramreelsrecommendedget) | **GET** /instagram/reels/recommended | Browse Instagram&#39;s recommended Reels feed |
| [**InstagramResolveMediaIdGet**](InstagramApi.md#instagramresolvemediaidget) | **GET** /instagram/resolve/media-id | Convert an Instagram post shortcode into its numeric media_id |
| [**InstagramResolveShortcodeFromMediaGet**](InstagramApi.md#instagramresolveshortcodefrommediaget) | **GET** /instagram/resolve/shortcode-from-media | Convert an Instagram numeric media_id into its shortcode |
| [**InstagramResolveShortcodeGet**](InstagramApi.md#instagramresolveshortcodeget) | **GET** /instagram/resolve/shortcode | Extract a post shortcode from an Instagram URL |
| [**InstagramResolveUserIdGet**](InstagramApi.md#instagramresolveuseridget) | **GET** /instagram/resolve/user-id | Convert an Instagram username into its numeric user_id (pk) |
| [**InstagramSearchGet**](InstagramApi.md#instagramsearchget) | **GET** /instagram/search | Cross-type Instagram search (posts/reels) |
| [**InstagramUsersUsernameFollowersGet**](InstagramApi.md#instagramusersusernamefollowersget) | **GET** /instagram/users/{username}/followers | List followers of an Instagram user |
| [**InstagramUsersUsernameFollowingGet**](InstagramApi.md#instagramusersusernamefollowingget) | **GET** /instagram/users/{username}/following | List accounts an Instagram user follows |
| [**InstagramUsersUsernameFormerUsernamesGet**](InstagramApi.md#instagramusersusernameformerusernamesget) | **GET** /instagram/users/{username}/former-usernames | List former usernames for an Instagram user |
| [**InstagramUsersUsernameGet**](InstagramApi.md#instagramusersusernameget) | **GET** /instagram/users/{username} | Get an Instagram user profile by username |
| [**InstagramUsersUsernameHighlightsGet**](InstagramApi.md#instagramusersusernamehighlightsget) | **GET** /instagram/users/{username}/highlights | List Instagram highlight reels for a user (metadata only) |
| [**InstagramUsersUsernamePostsGet**](InstagramApi.md#instagramusersusernamepostsget) | **GET** /instagram/users/{username}/posts | List feed posts authored by an Instagram user |
| [**InstagramUsersUsernameReelsGet**](InstagramApi.md#instagramusersusernamereelsget) | **GET** /instagram/users/{username}/reels | List reels authored by an Instagram user |
| [**InstagramUsersUsernameStoriesGet**](InstagramApi.md#instagramusersusernamestoriesget) | **GET** /instagram/users/{username}/stories | List active Instagram stories for a user |
| [**InstagramUsersUsernameTaggedPostsGet**](InstagramApi.md#instagramusersusernametaggedpostsget) | **GET** /instagram/users/{username}/tagged-posts | List posts an Instagram user is tagged in |

<a id="instagramexploreget"></a>
# **InstagramExploreGet**
> InstagramExploreGet200Response InstagramExploreGet (string? cursor = null)

Browse Instagram's Explore feed

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramExploreGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // Browse Instagram's Explore feed
                InstagramExploreGet200Response result = apiInstance.InstagramExploreGet(cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramExploreGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramExploreGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Browse Instagram's Explore feed
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramExploreGetWithHttpInfo(cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramExploreGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

<a id="instagramlocationsidget"></a>
# **InstagramLocationsIdGet**
> InstagramLocationsIdGet200Response InstagramLocationsIdGet (string id)

Get an Instagram location by id

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramLocationsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var id = "id_example";  // string | Numeric Instagram location id.

            try
            {
                // Get an Instagram location by id
                InstagramLocationsIdGet200Response result = apiInstance.InstagramLocationsIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramLocationsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramLocationsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get an Instagram location by id
    ApiResponse<InstagramLocationsIdGet200Response> response = apiInstance.InstagramLocationsIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramLocationsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | Numeric Instagram location id. |  |

### Return type

[**InstagramLocationsIdGet200Response**](InstagramLocationsIdGet200Response.md)

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

<a id="instagramlocationsidnearbyget"></a>
# **InstagramLocationsIdNearbyGet**
> InstagramLocationsIdNearbyGet200Response InstagramLocationsIdNearbyGet (string id)

List Instagram locations geographically near a given location

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramLocationsIdNearbyGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var id = "id_example";  // string | 

            try
            {
                // List Instagram locations geographically near a given location
                InstagramLocationsIdNearbyGet200Response result = apiInstance.InstagramLocationsIdNearbyGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramLocationsIdNearbyGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramLocationsIdNearbyGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Instagram locations geographically near a given location
    ApiResponse<InstagramLocationsIdNearbyGet200Response> response = apiInstance.InstagramLocationsIdNearbyGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramLocationsIdNearbyGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**InstagramLocationsIdNearbyGet200Response**](InstagramLocationsIdNearbyGet200Response.md)

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

<a id="instagramlocationsidpostsget"></a>
# **InstagramLocationsIdPostsGet**
> InstagramExploreGet200Response InstagramLocationsIdPostsGet (string id, string? cursor = null, string? tab = null)

List posts tagged with an Instagram location

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramLocationsIdPostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var tab = "ranked";  // string? | Which tab to fetch — `ranked` (top) or `recent` (latest). (optional) 

            try
            {
                // List posts tagged with an Instagram location
                InstagramExploreGet200Response result = apiInstance.InstagramLocationsIdPostsGet(id, cursor, tab);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramLocationsIdPostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramLocationsIdPostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List posts tagged with an Instagram location
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramLocationsIdPostsGetWithHttpInfo(id, cursor, tab);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramLocationsIdPostsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **tab** | **string?** | Which tab to fetch — &#x60;ranked&#x60; (top) or &#x60;recent&#x60; (latest). | [optional]  |

### Return type

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

<a id="instagrampostsshortcodecommentscommentidrepliesget"></a>
# **InstagramPostsShortcodeCommentsCommentIdRepliesGet**
> InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response InstagramPostsShortcodeCommentsCommentIdRepliesGet (string shortcode, string commentId, string? cursor = null)

List replies to an Instagram comment

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramPostsShortcodeCommentsCommentIdRepliesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var shortcode = "shortcode_example";  // string | 
            var commentId = "commentId_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List replies to an Instagram comment
                InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response result = apiInstance.InstagramPostsShortcodeCommentsCommentIdRepliesGet(shortcode, commentId, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramPostsShortcodeCommentsCommentIdRepliesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramPostsShortcodeCommentsCommentIdRepliesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List replies to an Instagram comment
    ApiResponse<InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response> response = apiInstance.InstagramPostsShortcodeCommentsCommentIdRepliesGetWithHttpInfo(shortcode, commentId, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramPostsShortcodeCommentsCommentIdRepliesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **shortcode** | **string** |  |  |
| **commentId** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response**](InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response.md)

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

<a id="instagrampostsshortcodecommentsget"></a>
# **InstagramPostsShortcodeCommentsGet**
> InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response InstagramPostsShortcodeCommentsGet (string shortcode, string? cursor = null, string? sort = null)

List comments on an Instagram post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramPostsShortcodeCommentsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var shortcode = "shortcode_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var sort = "popular";  // string? |  (optional) 

            try
            {
                // List comments on an Instagram post
                InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response result = apiInstance.InstagramPostsShortcodeCommentsGet(shortcode, cursor, sort);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramPostsShortcodeCommentsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramPostsShortcodeCommentsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List comments on an Instagram post
    ApiResponse<InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response> response = apiInstance.InstagramPostsShortcodeCommentsGetWithHttpInfo(shortcode, cursor, sort);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramPostsShortcodeCommentsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **shortcode** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **sort** | **string?** |  | [optional]  |

### Return type

[**InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response**](InstagramPostsShortcodeCommentsCommentIdRepliesGet200Response.md)

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

<a id="instagrampostsshortcodeget"></a>
# **InstagramPostsShortcodeGet**
> InstagramPostsShortcodeGet200Response InstagramPostsShortcodeGet (string shortcode)

Get an Instagram post (photo / video / carousel / reel) by shortcode

`shortcode` is the slug from the post URL, e.g. `DUajw4YkorV` in `instagram.com/p/DUajw4YkorV/`.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramPostsShortcodeGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var shortcode = "shortcode_example";  // string | 

            try
            {
                // Get an Instagram post (photo / video / carousel / reel) by shortcode
                InstagramPostsShortcodeGet200Response result = apiInstance.InstagramPostsShortcodeGet(shortcode);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramPostsShortcodeGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramPostsShortcodeGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get an Instagram post (photo / video / carousel / reel) by shortcode
    ApiResponse<InstagramPostsShortcodeGet200Response> response = apiInstance.InstagramPostsShortcodeGetWithHttpInfo(shortcode);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramPostsShortcodeGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **shortcode** | **string** |  |  |

### Return type

[**InstagramPostsShortcodeGet200Response**](InstagramPostsShortcodeGet200Response.md)

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

<a id="instagramreelsrecommendedget"></a>
# **InstagramReelsRecommendedGet**
> InstagramExploreGet200Response InstagramReelsRecommendedGet (string? cursor = null)

Browse Instagram's recommended Reels feed

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramReelsRecommendedGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // Browse Instagram's recommended Reels feed
                InstagramExploreGet200Response result = apiInstance.InstagramReelsRecommendedGet(cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramReelsRecommendedGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramReelsRecommendedGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Browse Instagram's recommended Reels feed
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramReelsRecommendedGetWithHttpInfo(cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramReelsRecommendedGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

<a id="instagramresolvemediaidget"></a>
# **InstagramResolveMediaIdGet**
> InstagramResolveMediaIdGet200Response InstagramResolveMediaIdGet (string shortcode)

Convert an Instagram post shortcode into its numeric media_id

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramResolveMediaIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var shortcode = "shortcode_example";  // string | 

            try
            {
                // Convert an Instagram post shortcode into its numeric media_id
                InstagramResolveMediaIdGet200Response result = apiInstance.InstagramResolveMediaIdGet(shortcode);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramResolveMediaIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramResolveMediaIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Convert an Instagram post shortcode into its numeric media_id
    ApiResponse<InstagramResolveMediaIdGet200Response> response = apiInstance.InstagramResolveMediaIdGetWithHttpInfo(shortcode);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramResolveMediaIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **shortcode** | **string** |  |  |

### Return type

[**InstagramResolveMediaIdGet200Response**](InstagramResolveMediaIdGet200Response.md)

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

<a id="instagramresolveshortcodefrommediaget"></a>
# **InstagramResolveShortcodeFromMediaGet**
> InstagramResolveMediaIdGet200Response InstagramResolveShortcodeFromMediaGet (string mediaId)

Convert an Instagram numeric media_id into its shortcode

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramResolveShortcodeFromMediaGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var mediaId = "mediaId_example";  // string | 

            try
            {
                // Convert an Instagram numeric media_id into its shortcode
                InstagramResolveMediaIdGet200Response result = apiInstance.InstagramResolveShortcodeFromMediaGet(mediaId);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramResolveShortcodeFromMediaGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramResolveShortcodeFromMediaGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Convert an Instagram numeric media_id into its shortcode
    ApiResponse<InstagramResolveMediaIdGet200Response> response = apiInstance.InstagramResolveShortcodeFromMediaGetWithHttpInfo(mediaId);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramResolveShortcodeFromMediaGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **mediaId** | **string** |  |  |

### Return type

[**InstagramResolveMediaIdGet200Response**](InstagramResolveMediaIdGet200Response.md)

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

<a id="instagramresolveshortcodeget"></a>
# **InstagramResolveShortcodeGet**
> InstagramResolveShortcodeGet200Response InstagramResolveShortcodeGet (string url)

Extract a post shortcode from an Instagram URL

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramResolveShortcodeGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var url = "url_example";  // string | 

            try
            {
                // Extract a post shortcode from an Instagram URL
                InstagramResolveShortcodeGet200Response result = apiInstance.InstagramResolveShortcodeGet(url);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramResolveShortcodeGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramResolveShortcodeGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Extract a post shortcode from an Instagram URL
    ApiResponse<InstagramResolveShortcodeGet200Response> response = apiInstance.InstagramResolveShortcodeGetWithHttpInfo(url);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramResolveShortcodeGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **url** | **string** |  |  |

### Return type

[**InstagramResolveShortcodeGet200Response**](InstagramResolveShortcodeGet200Response.md)

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

<a id="instagramresolveuseridget"></a>
# **InstagramResolveUserIdGet**
> InstagramResolveUserIdGet200Response InstagramResolveUserIdGet (string username)

Convert an Instagram username into its numeric user_id (pk)

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramResolveUserIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 

            try
            {
                // Convert an Instagram username into its numeric user_id (pk)
                InstagramResolveUserIdGet200Response result = apiInstance.InstagramResolveUserIdGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramResolveUserIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramResolveUserIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Convert an Instagram username into its numeric user_id (pk)
    ApiResponse<InstagramResolveUserIdGet200Response> response = apiInstance.InstagramResolveUserIdGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramResolveUserIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |

### Return type

[**InstagramResolveUserIdGet200Response**](InstagramResolveUserIdGet200Response.md)

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

<a id="instagramsearchget"></a>
# **InstagramSearchGet**
> InstagramExploreGet200Response InstagramSearchGet (string q, string? cursor = null)

Cross-type Instagram search (posts/reels)

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramSearchGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var q = "q_example";  // string | Search keyword.
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // Cross-type Instagram search (posts/reels)
                InstagramExploreGet200Response result = apiInstance.InstagramSearchGet(q, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramSearchGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramSearchGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Cross-type Instagram search (posts/reels)
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramSearchGetWithHttpInfo(q, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramSearchGetWithHttpInfo: " + e.Message);
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

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

<a id="instagramusersusernamefollowersget"></a>
# **InstagramUsersUsernameFollowersGet**
> InstagramUsersUsernameFollowersGet200Response InstagramUsersUsernameFollowersGet (string username, string? cursor = null)

List followers of an Instagram user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameFollowersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List followers of an Instagram user
                InstagramUsersUsernameFollowersGet200Response result = apiInstance.InstagramUsersUsernameFollowersGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameFollowersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameFollowersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List followers of an Instagram user
    ApiResponse<InstagramUsersUsernameFollowersGet200Response> response = apiInstance.InstagramUsersUsernameFollowersGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameFollowersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramUsersUsernameFollowersGet200Response**](InstagramUsersUsernameFollowersGet200Response.md)

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

<a id="instagramusersusernamefollowingget"></a>
# **InstagramUsersUsernameFollowingGet**
> InstagramUsersUsernameFollowersGet200Response InstagramUsersUsernameFollowingGet (string username, string? cursor = null)

List accounts an Instagram user follows

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameFollowingGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List accounts an Instagram user follows
                InstagramUsersUsernameFollowersGet200Response result = apiInstance.InstagramUsersUsernameFollowingGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameFollowingGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameFollowingGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List accounts an Instagram user follows
    ApiResponse<InstagramUsersUsernameFollowersGet200Response> response = apiInstance.InstagramUsersUsernameFollowingGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameFollowingGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramUsersUsernameFollowersGet200Response**](InstagramUsersUsernameFollowersGet200Response.md)

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

<a id="instagramusersusernameformerusernamesget"></a>
# **InstagramUsersUsernameFormerUsernamesGet**
> InstagramUsersUsernameFormerUsernamesGet200Response InstagramUsersUsernameFormerUsernamesGet (string username)

List former usernames for an Instagram user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameFormerUsernamesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 

            try
            {
                // List former usernames for an Instagram user
                InstagramUsersUsernameFormerUsernamesGet200Response result = apiInstance.InstagramUsersUsernameFormerUsernamesGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameFormerUsernamesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameFormerUsernamesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List former usernames for an Instagram user
    ApiResponse<InstagramUsersUsernameFormerUsernamesGet200Response> response = apiInstance.InstagramUsersUsernameFormerUsernamesGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameFormerUsernamesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |

### Return type

[**InstagramUsersUsernameFormerUsernamesGet200Response**](InstagramUsersUsernameFormerUsernamesGet200Response.md)

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

<a id="instagramusersusernameget"></a>
# **InstagramUsersUsernameGet**
> InstagramUsersUsernameGet200Response InstagramUsersUsernameGet (string username)

Get an Instagram user profile by username

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | Instagram URL slug, e.g. `instagram`

            try
            {
                // Get an Instagram user profile by username
                InstagramUsersUsernameGet200Response result = apiInstance.InstagramUsersUsernameGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get an Instagram user profile by username
    ApiResponse<InstagramUsersUsernameGet200Response> response = apiInstance.InstagramUsersUsernameGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** | Instagram URL slug, e.g. &#x60;instagram&#x60; |  |

### Return type

[**InstagramUsersUsernameGet200Response**](InstagramUsersUsernameGet200Response.md)

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

<a id="instagramusersusernamehighlightsget"></a>
# **InstagramUsersUsernameHighlightsGet**
> InstagramUsersUsernameHighlightsGet200Response InstagramUsersUsernameHighlightsGet (string username, string? cursor = null)

List Instagram highlight reels for a user (metadata only)

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameHighlightsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List Instagram highlight reels for a user (metadata only)
                InstagramUsersUsernameHighlightsGet200Response result = apiInstance.InstagramUsersUsernameHighlightsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameHighlightsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameHighlightsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Instagram highlight reels for a user (metadata only)
    ApiResponse<InstagramUsersUsernameHighlightsGet200Response> response = apiInstance.InstagramUsersUsernameHighlightsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameHighlightsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramUsersUsernameHighlightsGet200Response**](InstagramUsersUsernameHighlightsGet200Response.md)

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

<a id="instagramusersusernamepostsget"></a>
# **InstagramUsersUsernamePostsGet**
> InstagramExploreGet200Response InstagramUsersUsernamePostsGet (string username, string? cursor = null)

List feed posts authored by an Instagram user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernamePostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List feed posts authored by an Instagram user
                InstagramExploreGet200Response result = apiInstance.InstagramUsersUsernamePostsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernamePostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernamePostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List feed posts authored by an Instagram user
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramUsersUsernamePostsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernamePostsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

<a id="instagramusersusernamereelsget"></a>
# **InstagramUsersUsernameReelsGet**
> InstagramExploreGet200Response InstagramUsersUsernameReelsGet (string username, string? cursor = null)

List reels authored by an Instagram user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameReelsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List reels authored by an Instagram user
                InstagramExploreGet200Response result = apiInstance.InstagramUsersUsernameReelsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameReelsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameReelsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List reels authored by an Instagram user
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramUsersUsernameReelsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameReelsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

<a id="instagramusersusernamestoriesget"></a>
# **InstagramUsersUsernameStoriesGet**
> InstagramExploreGet200Response InstagramUsersUsernameStoriesGet (string username)

List active Instagram stories for a user

Returns the user's currently-live story tray (empty when the user has no active stories).

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameStoriesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 

            try
            {
                // List active Instagram stories for a user
                InstagramExploreGet200Response result = apiInstance.InstagramUsersUsernameStoriesGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameStoriesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameStoriesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List active Instagram stories for a user
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramUsersUsernameStoriesGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameStoriesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |

### Return type

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

<a id="instagramusersusernametaggedpostsget"></a>
# **InstagramUsersUsernameTaggedPostsGet**
> InstagramExploreGet200Response InstagramUsersUsernameTaggedPostsGet (string username, string? cursor = null)

List posts an Instagram user is tagged in

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class InstagramUsersUsernameTaggedPostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new InstagramApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List posts an Instagram user is tagged in
                InstagramExploreGet200Response result = apiInstance.InstagramUsersUsernameTaggedPostsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameTaggedPostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the InstagramUsersUsernameTaggedPostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List posts an Instagram user is tagged in
    ApiResponse<InstagramExploreGet200Response> response = apiInstance.InstagramUsersUsernameTaggedPostsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling InstagramApi.InstagramUsersUsernameTaggedPostsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**InstagramExploreGet200Response**](InstagramExploreGet200Response.md)

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

