# Unifapi.Sdk.Api.XApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**XAutocompleteGet**](XApi.md#xautocompleteget) | **GET** /x/autocomplete | Autocomplete X users, topics, hashtags, and cashtags |
| [**XCommunitiesIdAboutGet**](XApi.md#xcommunitiesidaboutget) | **GET** /x/communities/{id}/about | Get an X Community about timeline |
| [**XCommunitiesIdGet**](XApi.md#xcommunitiesidget) | **GET** /x/communities/{id} | Get X Community by ID |
| [**XCommunitiesIdMediaGet**](XApi.md#xcommunitiesidmediaget) | **GET** /x/communities/{id}/media | Get media Posts from an X Community |
| [**XCommunitiesIdMemberSearchGet**](XApi.md#xcommunitiesidmembersearchget) | **GET** /x/communities/{id}/member_search | Search members in an X Community |
| [**XCommunitiesIdMembersGet**](XApi.md#xcommunitiesidmembersget) | **GET** /x/communities/{id}/members | Get members of an X Community |
| [**XCommunitiesIdModeratorsGet**](XApi.md#xcommunitiesidmoderatorsget) | **GET** /x/communities/{id}/moderators | Get moderators of an X Community |
| [**XCommunitiesIdTweetsGet**](XApi.md#xcommunitiesidtweetsget) | **GET** /x/communities/{id}/tweets | Get Posts from an X Community |
| [**XCommunitiesSearchGet**](XApi.md#xcommunitiessearchget) | **GET** /x/communities/search | Search X Communities |
| [**XFriendshipsShowGet**](XApi.md#xfriendshipsshowget) | **GET** /x/friendships/show | Check whether one X user follows another |
| [**XListsIdFollowersGet**](XApi.md#xlistsidfollowersget) | **GET** /x/lists/{id}/followers | Get followers/subscribers of an X List |
| [**XListsIdMembersGet**](XApi.md#xlistsidmembersget) | **GET** /x/lists/{id}/members | Get members of an X List |
| [**XListsIdTweetsGet**](XApi.md#xlistsidtweetsget) | **GET** /x/lists/{id}/tweets | Get Posts from an X List |
| [**XListsSearchGet**](XApi.md#xlistssearchget) | **GET** /x/lists/search | Search X Lists |
| [**XTrendsByWoeidWoeidGet**](XApi.md#xtrendsbywoeidwoeidget) | **GET** /x/trends/by/woeid/{woeid} | Get X trends by WOEID |
| [**XTweetsGet**](XApi.md#xtweetsget) | **GET** /x/tweets | Get X Posts by IDs |
| [**XTweetsIdArticleGet**](XApi.md#xtweetsidarticleget) | **GET** /x/tweets/{id}/article | Get the article-style payload for an X Post |
| [**XTweetsIdGet**](XApi.md#xtweetsidget) | **GET** /x/tweets/{id} | Get X Post by ID |
| [**XTweetsIdLikingUsersGet**](XApi.md#xtweetsidlikingusersget) | **GET** /x/tweets/{id}/liking_users | Get users who liked an X Post |
| [**XTweetsIdQuoteTweetsGet**](XApi.md#xtweetsidquotetweetsget) | **GET** /x/tweets/{id}/quote_tweets | Get quote Posts for an X Post |
| [**XTweetsIdRetweetedByGet**](XApi.md#xtweetsidretweetedbyget) | **GET** /x/tweets/{id}/retweeted_by | Get users who reposted an X Post |
| [**XTweetsIdTranslationGet**](XApi.md#xtweetsidtranslationget) | **GET** /x/tweets/{id}/translation | Translate an X Post |
| [**XTweetsSearchRecentGet**](XApi.md#xtweetssearchrecentget) | **GET** /x/tweets/search/recent | Search recent X Posts |
| [**XUsersByGet**](XApi.md#xusersbyget) | **GET** /x/users/by | Get X users by usernames |
| [**XUsersByUsernameUsernameGet**](XApi.md#xusersbyusernameusernameget) | **GET** /x/users/by/username/{username} | Get X user by username |
| [**XUsersGet**](XApi.md#xusersget) | **GET** /x/users | Get X users by IDs |
| [**XUsersIdFollowersGet**](XApi.md#xusersidfollowersget) | **GET** /x/users/{id}/followers | Get an X user&#39;s followers |
| [**XUsersIdFollowersIdsGet**](XApi.md#xusersidfollowersidsget) | **GET** /x/users/{id}/followers/ids | Get follower IDs for an X user |
| [**XUsersIdFollowingGet**](XApi.md#xusersidfollowingget) | **GET** /x/users/{id}/following | Get users followed by an X user |
| [**XUsersIdFollowingIdsGet**](XApi.md#xusersidfollowingidsget) | **GET** /x/users/{id}/following/ids | Get following IDs for an X user |
| [**XUsersIdGet**](XApi.md#xusersidget) | **GET** /x/users/{id} | Get X user by ID |
| [**XUsersIdLikedTweetsGet**](XApi.md#xusersidlikedtweetsget) | **GET** /x/users/{id}/liked_tweets | Get Posts liked by an X user |
| [**XUsersIdProfileTranslationGet**](XApi.md#xusersidprofiletranslationget) | **GET** /x/users/{id}/profile_translation | Translate an X user profile |
| [**XUsersIdTweetsGet**](XApi.md#xusersidtweetsget) | **GET** /x/users/{id}/tweets | Get Posts authored by an X user |
| [**XUsersIdVerifiedFollowersGet**](XApi.md#xusersidverifiedfollowersget) | **GET** /x/users/{id}/verified_followers | Get verified followers for an X user |

<a id="xautocompleteget"></a>
# **XAutocompleteGet**
> XAutocompleteGet200Response XAutocompleteGet (string query)

Autocomplete X users, topics, hashtags, and cashtags

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XAutocompleteGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var query = "query_example";  // string | 

            try
            {
                // Autocomplete X users, topics, hashtags, and cashtags
                XAutocompleteGet200Response result = apiInstance.XAutocompleteGet(query);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XAutocompleteGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XAutocompleteGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Autocomplete X users, topics, hashtags, and cashtags
    ApiResponse<XAutocompleteGet200Response> response = apiInstance.XAutocompleteGetWithHttpInfo(query);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XAutocompleteGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **query** | **string** |  |  |

### Return type

[**XAutocompleteGet200Response**](XAutocompleteGet200Response.md)

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

<a id="xcommunitiesidaboutget"></a>
# **XCommunitiesIdAboutGet**
> XCommunitiesIdAboutGet200Response XCommunitiesIdAboutGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get an X Community about timeline

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesIdAboutGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get an X Community about timeline
                XCommunitiesIdAboutGet200Response result = apiInstance.XCommunitiesIdAboutGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesIdAboutGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesIdAboutGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get an X Community about timeline
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XCommunitiesIdAboutGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesIdAboutGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xcommunitiesidget"></a>
# **XCommunitiesIdGet**
> XCommunitiesIdGet200Response XCommunitiesIdGet (string id, string? communityFields = null)

Get X Community by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var communityFields = "communityFields_example";  // string? |  (optional) 

            try
            {
                // Get X Community by ID
                XCommunitiesIdGet200Response result = apiInstance.XCommunitiesIdGet(id, communityFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X Community by ID
    ApiResponse<XCommunitiesIdGet200Response> response = apiInstance.XCommunitiesIdGetWithHttpInfo(id, communityFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **communityFields** | **string?** |  | [optional]  |

### Return type

[**XCommunitiesIdGet200Response**](XCommunitiesIdGet200Response.md)

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

<a id="xcommunitiesidmediaget"></a>
# **XCommunitiesIdMediaGet**
> XCommunitiesIdAboutGet200Response XCommunitiesIdMediaGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get media Posts from an X Community

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesIdMediaGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get media Posts from an X Community
                XCommunitiesIdAboutGet200Response result = apiInstance.XCommunitiesIdMediaGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesIdMediaGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesIdMediaGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get media Posts from an X Community
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XCommunitiesIdMediaGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesIdMediaGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xcommunitiesidmembersearchget"></a>
# **XCommunitiesIdMemberSearchGet**
> XCommunitiesIdMemberSearchGet200Response XCommunitiesIdMemberSearchGet (string id, string query, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Search members in an X Community

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesIdMemberSearchGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var query = "query_example";  // string | 
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Search members in an X Community
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XCommunitiesIdMemberSearchGet(id, query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesIdMemberSearchGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesIdMemberSearchGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search members in an X Community
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XCommunitiesIdMemberSearchGetWithHttpInfo(id, query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesIdMemberSearchGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **query** | **string** |  |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xcommunitiesidmembersget"></a>
# **XCommunitiesIdMembersGet**
> XCommunitiesIdMemberSearchGet200Response XCommunitiesIdMembersGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get members of an X Community

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesIdMembersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get members of an X Community
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XCommunitiesIdMembersGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesIdMembersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesIdMembersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get members of an X Community
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XCommunitiesIdMembersGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesIdMembersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xcommunitiesidmoderatorsget"></a>
# **XCommunitiesIdModeratorsGet**
> XCommunitiesIdMemberSearchGet200Response XCommunitiesIdModeratorsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get moderators of an X Community

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesIdModeratorsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get moderators of an X Community
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XCommunitiesIdModeratorsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesIdModeratorsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesIdModeratorsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get moderators of an X Community
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XCommunitiesIdModeratorsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesIdModeratorsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xcommunitiesidtweetsget"></a>
# **XCommunitiesIdTweetsGet**
> XCommunitiesIdAboutGet200Response XCommunitiesIdTweetsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get Posts from an X Community

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesIdTweetsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get Posts from an X Community
                XCommunitiesIdAboutGet200Response result = apiInstance.XCommunitiesIdTweetsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesIdTweetsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesIdTweetsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get Posts from an X Community
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XCommunitiesIdTweetsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesIdTweetsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xcommunitiessearchget"></a>
# **XCommunitiesSearchGet**
> XCommunitiesSearchGet200Response XCommunitiesSearchGet (string query, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null, string? communityFields = null)

Search X Communities

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XCommunitiesSearchGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var query = "query_example";  // string | 
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 
            var communityFields = "communityFields_example";  // string? |  (optional) 

            try
            {
                // Search X Communities
                XCommunitiesSearchGet200Response result = apiInstance.XCommunitiesSearchGet(query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults, communityFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XCommunitiesSearchGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XCommunitiesSearchGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search X Communities
    ApiResponse<XCommunitiesSearchGet200Response> response = apiInstance.XCommunitiesSearchGetWithHttpInfo(query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults, communityFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XCommunitiesSearchGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **query** | **string** |  |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |
| **communityFields** | **string?** |  | [optional]  |

### Return type

[**XCommunitiesSearchGet200Response**](XCommunitiesSearchGet200Response.md)

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

<a id="xfriendshipsshowget"></a>
# **XFriendshipsShowGet**
> XFriendshipsShowGet200Response XFriendshipsShowGet (string? sourceId = null, string? targetId = null, string? sourceScreenName = null, string? targetScreenName = null)

Check whether one X user follows another

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XFriendshipsShowGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var sourceId = "sourceId_example";  // string? |  (optional) 
            var targetId = "targetId_example";  // string? |  (optional) 
            var sourceScreenName = "sourceScreenName_example";  // string? |  (optional) 
            var targetScreenName = "targetScreenName_example";  // string? |  (optional) 

            try
            {
                // Check whether one X user follows another
                XFriendshipsShowGet200Response result = apiInstance.XFriendshipsShowGet(sourceId, targetId, sourceScreenName, targetScreenName);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XFriendshipsShowGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XFriendshipsShowGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Check whether one X user follows another
    ApiResponse<XFriendshipsShowGet200Response> response = apiInstance.XFriendshipsShowGetWithHttpInfo(sourceId, targetId, sourceScreenName, targetScreenName);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XFriendshipsShowGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **sourceId** | **string?** |  | [optional]  |
| **targetId** | **string?** |  | [optional]  |
| **sourceScreenName** | **string?** |  | [optional]  |
| **targetScreenName** | **string?** |  | [optional]  |

### Return type

[**XFriendshipsShowGet200Response**](XFriendshipsShowGet200Response.md)

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

<a id="xlistsidfollowersget"></a>
# **XListsIdFollowersGet**
> XCommunitiesIdMemberSearchGet200Response XListsIdFollowersGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get followers/subscribers of an X List

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XListsIdFollowersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get followers/subscribers of an X List
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XListsIdFollowersGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XListsIdFollowersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XListsIdFollowersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get followers/subscribers of an X List
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XListsIdFollowersGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XListsIdFollowersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xlistsidmembersget"></a>
# **XListsIdMembersGet**
> XCommunitiesIdMemberSearchGet200Response XListsIdMembersGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get members of an X List

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XListsIdMembersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get members of an X List
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XListsIdMembersGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XListsIdMembersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XListsIdMembersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get members of an X List
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XListsIdMembersGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XListsIdMembersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xlistsidtweetsget"></a>
# **XListsIdTweetsGet**
> XCommunitiesIdAboutGet200Response XListsIdTweetsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get Posts from an X List

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XListsIdTweetsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get Posts from an X List
                XCommunitiesIdAboutGet200Response result = apiInstance.XListsIdTweetsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XListsIdTweetsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XListsIdTweetsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get Posts from an X List
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XListsIdTweetsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XListsIdTweetsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xlistssearchget"></a>
# **XListsSearchGet**
> XListsSearchGet200Response XListsSearchGet (string query, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Search X Lists

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XListsSearchGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var query = "query_example";  // string | 
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Search X Lists
                XListsSearchGet200Response result = apiInstance.XListsSearchGet(query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XListsSearchGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XListsSearchGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search X Lists
    ApiResponse<XListsSearchGet200Response> response = apiInstance.XListsSearchGetWithHttpInfo(query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XListsSearchGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **query** | **string** |  |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XListsSearchGet200Response**](XListsSearchGet200Response.md)

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

<a id="xtrendsbywoeidwoeidget"></a>
# **XTrendsByWoeidWoeidGet**
> XTrendsByWoeidWoeidGet200Response XTrendsByWoeidWoeidGet (string woeid, int? maxTrends = null, string? trendFields = null)

Get X trends by WOEID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTrendsByWoeidWoeidGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var woeid = "woeid_example";  // string | 
            var maxTrends = 56;  // int? |  (optional) 
            var trendFields = "trendFields_example";  // string? |  (optional) 

            try
            {
                // Get X trends by WOEID
                XTrendsByWoeidWoeidGet200Response result = apiInstance.XTrendsByWoeidWoeidGet(woeid, maxTrends, trendFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTrendsByWoeidWoeidGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTrendsByWoeidWoeidGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X trends by WOEID
    ApiResponse<XTrendsByWoeidWoeidGet200Response> response = apiInstance.XTrendsByWoeidWoeidGetWithHttpInfo(woeid, maxTrends, trendFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTrendsByWoeidWoeidGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **woeid** | **string** |  |  |
| **maxTrends** | **int?** |  | [optional]  |
| **trendFields** | **string?** |  | [optional]  |

### Return type

[**XTrendsByWoeidWoeidGet200Response**](XTrendsByWoeidWoeidGet200Response.md)

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

<a id="xtweetsget"></a>
# **XTweetsGet**
> XTweetsGet200Response XTweetsGet (string ids, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null)

Get X Posts by IDs

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var ids = "ids_example";  // string | Comma-separated resource ids.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 

            try
            {
                // Get X Posts by IDs
                XTweetsGet200Response result = apiInstance.XTweetsGet(ids, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X Posts by IDs
    ApiResponse<XTweetsGet200Response> response = apiInstance.XTweetsGetWithHttpInfo(ids, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **ids** | **string** | Comma-separated resource ids. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |

### Return type

[**XTweetsGet200Response**](XTweetsGet200Response.md)

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

<a id="xtweetsidarticleget"></a>
# **XTweetsIdArticleGet**
> XTweetsIdArticleGet200Response XTweetsIdArticleGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null)

Get the article-style payload for an X Post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsIdArticleGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 

            try
            {
                // Get the article-style payload for an X Post
                XTweetsIdArticleGet200Response result = apiInstance.XTweetsIdArticleGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsIdArticleGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsIdArticleGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get the article-style payload for an X Post
    ApiResponse<XTweetsIdArticleGet200Response> response = apiInstance.XTweetsIdArticleGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsIdArticleGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |

### Return type

[**XTweetsIdArticleGet200Response**](XTweetsIdArticleGet200Response.md)

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

<a id="xtweetsidget"></a>
# **XTweetsIdGet**
> XTweetsIdGet200Response XTweetsIdGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null)

Get X Post by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 

            try
            {
                // Get X Post by ID
                XTweetsIdGet200Response result = apiInstance.XTweetsIdGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X Post by ID
    ApiResponse<XTweetsIdGet200Response> response = apiInstance.XTweetsIdGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |

### Return type

[**XTweetsIdGet200Response**](XTweetsIdGet200Response.md)

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

<a id="xtweetsidlikingusersget"></a>
# **XTweetsIdLikingUsersGet**
> XCommunitiesIdMemberSearchGet200Response XTweetsIdLikingUsersGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get users who liked an X Post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsIdLikingUsersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get users who liked an X Post
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XTweetsIdLikingUsersGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsIdLikingUsersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsIdLikingUsersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get users who liked an X Post
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XTweetsIdLikingUsersGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsIdLikingUsersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xtweetsidquotetweetsget"></a>
# **XTweetsIdQuoteTweetsGet**
> XCommunitiesIdAboutGet200Response XTweetsIdQuoteTweetsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get quote Posts for an X Post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsIdQuoteTweetsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get quote Posts for an X Post
                XCommunitiesIdAboutGet200Response result = apiInstance.XTweetsIdQuoteTweetsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsIdQuoteTweetsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsIdQuoteTweetsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get quote Posts for an X Post
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XTweetsIdQuoteTweetsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsIdQuoteTweetsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xtweetsidretweetedbyget"></a>
# **XTweetsIdRetweetedByGet**
> XCommunitiesIdMemberSearchGet200Response XTweetsIdRetweetedByGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get users who reposted an X Post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsIdRetweetedByGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get users who reposted an X Post
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XTweetsIdRetweetedByGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsIdRetweetedByGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsIdRetweetedByGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get users who reposted an X Post
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XTweetsIdRetweetedByGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsIdRetweetedByGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xtweetsidtranslationget"></a>
# **XTweetsIdTranslationGet**
> XTweetsIdTranslationGet200Response XTweetsIdTranslationGet (string id, string language)

Translate an X Post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsIdTranslationGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var language = "language_example";  // string | 

            try
            {
                // Translate an X Post
                XTweetsIdTranslationGet200Response result = apiInstance.XTweetsIdTranslationGet(id, language);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsIdTranslationGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsIdTranslationGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Translate an X Post
    ApiResponse<XTweetsIdTranslationGet200Response> response = apiInstance.XTweetsIdTranslationGetWithHttpInfo(id, language);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsIdTranslationGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **language** | **string** |  |  |

### Return type

[**XTweetsIdTranslationGet200Response**](XTweetsIdTranslationGet200Response.md)

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

<a id="xtweetssearchrecentget"></a>
# **XTweetsSearchRecentGet**
> XCommunitiesIdAboutGet200Response XTweetsSearchRecentGet (string query, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Search recent X Posts

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XTweetsSearchRecentGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var query = "query_example";  // string | Recent search query.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Search recent X Posts
                XCommunitiesIdAboutGet200Response result = apiInstance.XTweetsSearchRecentGet(query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XTweetsSearchRecentGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XTweetsSearchRecentGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search recent X Posts
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XTweetsSearchRecentGetWithHttpInfo(query, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XTweetsSearchRecentGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **query** | **string** | Recent search query. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xusersbyget"></a>
# **XUsersByGet**
> XUsersByGet200Response XUsersByGet (string usernames, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null)

Get X users by usernames

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersByGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var usernames = "usernames_example";  // string | Comma-separated usernames.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 

            try
            {
                // Get X users by usernames
                XUsersByGet200Response result = apiInstance.XUsersByGet(usernames, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersByGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersByGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X users by usernames
    ApiResponse<XUsersByGet200Response> response = apiInstance.XUsersByGetWithHttpInfo(usernames, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersByGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **usernames** | **string** | Comma-separated usernames. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |

### Return type

[**XUsersByGet200Response**](XUsersByGet200Response.md)

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

<a id="xusersbyusernameusernameget"></a>
# **XUsersByUsernameUsernameGet**
> XUsersIdGet200Response XUsersByUsernameUsernameGet (string username, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null)

Get X user by username

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersByUsernameUsernameGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var username = "username_example";  // string | X handle without the leading `@`.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 

            try
            {
                // Get X user by username
                XUsersIdGet200Response result = apiInstance.XUsersByUsernameUsernameGet(username, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersByUsernameUsernameGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersByUsernameUsernameGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X user by username
    ApiResponse<XUsersIdGet200Response> response = apiInstance.XUsersByUsernameUsernameGetWithHttpInfo(username, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersByUsernameUsernameGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** | X handle without the leading &#x60;@&#x60;. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |

### Return type

[**XUsersIdGet200Response**](XUsersIdGet200Response.md)

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

<a id="xusersget"></a>
# **XUsersGet**
> XUsersByGet200Response XUsersGet (string ids, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null)

Get X users by IDs

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var ids = "ids_example";  // string | Comma-separated resource ids.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 

            try
            {
                // Get X users by IDs
                XUsersByGet200Response result = apiInstance.XUsersGet(ids, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X users by IDs
    ApiResponse<XUsersByGet200Response> response = apiInstance.XUsersGetWithHttpInfo(ids, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **ids** | **string** | Comma-separated resource ids. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |

### Return type

[**XUsersByGet200Response**](XUsersByGet200Response.md)

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

<a id="xusersidfollowersget"></a>
# **XUsersIdFollowersGet**
> XCommunitiesIdMemberSearchGet200Response XUsersIdFollowersGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get an X user's followers

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdFollowersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get an X user's followers
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XUsersIdFollowersGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdFollowersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdFollowersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get an X user's followers
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XUsersIdFollowersGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdFollowersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xusersidfollowersidsget"></a>
# **XUsersIdFollowersIdsGet**
> XUsersIdFollowersIdsGet200Response XUsersIdFollowersIdsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get follower IDs for an X user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdFollowersIdsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get follower IDs for an X user
                XUsersIdFollowersIdsGet200Response result = apiInstance.XUsersIdFollowersIdsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdFollowersIdsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdFollowersIdsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get follower IDs for an X user
    ApiResponse<XUsersIdFollowersIdsGet200Response> response = apiInstance.XUsersIdFollowersIdsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdFollowersIdsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XUsersIdFollowersIdsGet200Response**](XUsersIdFollowersIdsGet200Response.md)

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

<a id="xusersidfollowingget"></a>
# **XUsersIdFollowingGet**
> XCommunitiesIdMemberSearchGet200Response XUsersIdFollowingGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get users followed by an X user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdFollowingGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get users followed by an X user
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XUsersIdFollowingGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdFollowingGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdFollowingGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get users followed by an X user
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XUsersIdFollowingGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdFollowingGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

<a id="xusersidfollowingidsget"></a>
# **XUsersIdFollowingIdsGet**
> XUsersIdFollowersIdsGet200Response XUsersIdFollowingIdsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get following IDs for an X user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdFollowingIdsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get following IDs for an X user
                XUsersIdFollowersIdsGet200Response result = apiInstance.XUsersIdFollowingIdsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdFollowingIdsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdFollowingIdsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get following IDs for an X user
    ApiResponse<XUsersIdFollowersIdsGet200Response> response = apiInstance.XUsersIdFollowingIdsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdFollowingIdsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XUsersIdFollowersIdsGet200Response**](XUsersIdFollowersIdsGet200Response.md)

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

<a id="xusersidget"></a>
# **XUsersIdGet**
> XUsersIdGet200Response XUsersIdGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null)

Get X user by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 

            try
            {
                // Get X user by ID
                XUsersIdGet200Response result = apiInstance.XUsersIdGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get X user by ID
    ApiResponse<XUsersIdGet200Response> response = apiInstance.XUsersIdGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |

### Return type

[**XUsersIdGet200Response**](XUsersIdGet200Response.md)

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

<a id="xusersidlikedtweetsget"></a>
# **XUsersIdLikedTweetsGet**
> XCommunitiesIdAboutGet200Response XUsersIdLikedTweetsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get Posts liked by an X user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdLikedTweetsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get Posts liked by an X user
                XCommunitiesIdAboutGet200Response result = apiInstance.XUsersIdLikedTweetsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdLikedTweetsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdLikedTweetsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get Posts liked by an X user
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XUsersIdLikedTweetsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdLikedTweetsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xusersidprofiletranslationget"></a>
# **XUsersIdProfileTranslationGet**
> XTweetsIdTranslationGet200Response XUsersIdProfileTranslationGet (string id, string language)

Translate an X user profile

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdProfileTranslationGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var language = "language_example";  // string | 

            try
            {
                // Translate an X user profile
                XTweetsIdTranslationGet200Response result = apiInstance.XUsersIdProfileTranslationGet(id, language);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdProfileTranslationGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdProfileTranslationGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Translate an X user profile
    ApiResponse<XTweetsIdTranslationGet200Response> response = apiInstance.XUsersIdProfileTranslationGetWithHttpInfo(id, language);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdProfileTranslationGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **language** | **string** |  |  |

### Return type

[**XTweetsIdTranslationGet200Response**](XTweetsIdTranslationGet200Response.md)

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

<a id="xusersidtweetsget"></a>
# **XUsersIdTweetsGet**
> XCommunitiesIdAboutGet200Response XUsersIdTweetsGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null, string? exclude = null)

Get Posts authored by an X user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdTweetsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 
            var exclude = "exclude_example";  // string? | Comma-separated X timeline exclusions, e.g. `replies`. (optional) 

            try
            {
                // Get Posts authored by an X user
                XCommunitiesIdAboutGet200Response result = apiInstance.XUsersIdTweetsGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults, exclude);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdTweetsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdTweetsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get Posts authored by an X user
    ApiResponse<XCommunitiesIdAboutGet200Response> response = apiInstance.XUsersIdTweetsGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults, exclude);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdTweetsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |
| **exclude** | **string?** | Comma-separated X timeline exclusions, e.g. &#x60;replies&#x60;. | [optional]  |

### Return type

[**XCommunitiesIdAboutGet200Response**](XCommunitiesIdAboutGet200Response.md)

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

<a id="xusersidverifiedfollowersget"></a>
# **XUsersIdVerifiedFollowersGet**
> XCommunitiesIdMemberSearchGet200Response XUsersIdVerifiedFollowersGet (string id, string? expansions = null, string? tweetFields = null, string? userFields = null, string? mediaFields = null, string? placeFields = null, string? pollFields = null, string? paginationToken = null, string? nextToken = null, int? maxResults = null)

Get verified followers for an X user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class XUsersIdVerifiedFollowersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new XApi(config);
            var id = "id_example";  // string | X resource id.
            var expansions = "expansions_example";  // string? |  (optional) 
            var tweetFields = "tweetFields_example";  // string? |  (optional) 
            var userFields = "userFields_example";  // string? |  (optional) 
            var mediaFields = "mediaFields_example";  // string? |  (optional) 
            var placeFields = "placeFields_example";  // string? |  (optional) 
            var pollFields = "pollFields_example";  // string? |  (optional) 
            var paginationToken = "paginationToken_example";  // string? |  (optional) 
            var nextToken = "nextToken_example";  // string? |  (optional) 
            var maxResults = 56;  // int? |  (optional) 

            try
            {
                // Get verified followers for an X user
                XCommunitiesIdMemberSearchGet200Response result = apiInstance.XUsersIdVerifiedFollowersGet(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling XApi.XUsersIdVerifiedFollowersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the XUsersIdVerifiedFollowersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get verified followers for an X user
    ApiResponse<XCommunitiesIdMemberSearchGet200Response> response = apiInstance.XUsersIdVerifiedFollowersGetWithHttpInfo(id, expansions, tweetFields, userFields, mediaFields, placeFields, pollFields, paginationToken, nextToken, maxResults);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling XApi.XUsersIdVerifiedFollowersGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** | X resource id. |  |
| **expansions** | **string?** |  | [optional]  |
| **tweetFields** | **string?** |  | [optional]  |
| **userFields** | **string?** |  | [optional]  |
| **mediaFields** | **string?** |  | [optional]  |
| **placeFields** | **string?** |  | [optional]  |
| **pollFields** | **string?** |  | [optional]  |
| **paginationToken** | **string?** |  | [optional]  |
| **nextToken** | **string?** |  | [optional]  |
| **maxResults** | **int?** |  | [optional]  |

### Return type

[**XCommunitiesIdMemberSearchGet200Response**](XCommunitiesIdMemberSearchGet200Response.md)

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

