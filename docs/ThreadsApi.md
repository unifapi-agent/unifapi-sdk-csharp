# Unifapi.Sdk.Api.ThreadsApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ThreadsSearchProfilesGet**](ThreadsApi.md#threadssearchprofilesget) | **GET** /threads/search/profiles | Search Threads users by keyword |
| [**ThreadsSearchRecentGet**](ThreadsApi.md#threadssearchrecentget) | **GET** /threads/search/recent | Search recent Threads posts |
| [**ThreadsSearchTopGet**](ThreadsApi.md#threadssearchtopget) | **GET** /threads/search/top | Search top Threads posts |
| [**ThreadsUsersUsernameGet**](ThreadsApi.md#threadsusersusernameget) | **GET** /threads/users/{username} | Get a Threads user profile by username |
| [**ThreadsUsersUsernamePostsGet**](ThreadsApi.md#threadsusersusernamepostsget) | **GET** /threads/users/{username}/posts | List Threads posts authored by a user |
| [**ThreadsUsersUsernameRepliesGet**](ThreadsApi.md#threadsusersusernamerepliesget) | **GET** /threads/users/{username}/replies | List Threads replies authored by a user |
| [**ThreadsUsersUsernameRepostsGet**](ThreadsApi.md#threadsusersusernamerepostsget) | **GET** /threads/users/{username}/reposts | List Threads reposts by a user |

<a id="threadssearchprofilesget"></a>
# **ThreadsSearchProfilesGet**
> ThreadsSearchProfilesGet200Response ThreadsSearchProfilesGet (string q)

Search Threads users by keyword

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class ThreadsSearchProfilesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new ThreadsApi(config);
            var q = "q_example";  // string | Search keyword.

            try
            {
                // Search Threads users by keyword
                ThreadsSearchProfilesGet200Response result = apiInstance.ThreadsSearchProfilesGet(q);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ThreadsApi.ThreadsSearchProfilesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ThreadsSearchProfilesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search Threads users by keyword
    ApiResponse<ThreadsSearchProfilesGet200Response> response = apiInstance.ThreadsSearchProfilesGetWithHttpInfo(q);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ThreadsApi.ThreadsSearchProfilesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **q** | **string** | Search keyword. |  |

### Return type

[**ThreadsSearchProfilesGet200Response**](ThreadsSearchProfilesGet200Response.md)

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

<a id="threadssearchrecentget"></a>
# **ThreadsSearchRecentGet**
> ThreadsSearchRecentGet200Response ThreadsSearchRecentGet (string q, string? cursor = null)

Search recent Threads posts

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class ThreadsSearchRecentGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new ThreadsApi(config);
            var q = "q_example";  // string | Search keyword.
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // Search recent Threads posts
                ThreadsSearchRecentGet200Response result = apiInstance.ThreadsSearchRecentGet(q, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ThreadsApi.ThreadsSearchRecentGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ThreadsSearchRecentGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search recent Threads posts
    ApiResponse<ThreadsSearchRecentGet200Response> response = apiInstance.ThreadsSearchRecentGetWithHttpInfo(q, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ThreadsApi.ThreadsSearchRecentGetWithHttpInfo: " + e.Message);
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

[**ThreadsSearchRecentGet200Response**](ThreadsSearchRecentGet200Response.md)

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

<a id="threadssearchtopget"></a>
# **ThreadsSearchTopGet**
> ThreadsSearchRecentGet200Response ThreadsSearchTopGet (string q, string? cursor = null)

Search top Threads posts

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class ThreadsSearchTopGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new ThreadsApi(config);
            var q = "q_example";  // string | Search keyword.
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // Search top Threads posts
                ThreadsSearchRecentGet200Response result = apiInstance.ThreadsSearchTopGet(q, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ThreadsApi.ThreadsSearchTopGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ThreadsSearchTopGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search top Threads posts
    ApiResponse<ThreadsSearchRecentGet200Response> response = apiInstance.ThreadsSearchTopGetWithHttpInfo(q, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ThreadsApi.ThreadsSearchTopGetWithHttpInfo: " + e.Message);
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

[**ThreadsSearchRecentGet200Response**](ThreadsSearchRecentGet200Response.md)

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

<a id="threadsusersusernameget"></a>
# **ThreadsUsersUsernameGet**
> ThreadsUsersUsernameGet200Response ThreadsUsersUsernameGet (string username)

Get a Threads user profile by username

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class ThreadsUsersUsernameGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new ThreadsApi(config);
            var username = "username_example";  // string | 

            try
            {
                // Get a Threads user profile by username
                ThreadsUsersUsernameGet200Response result = apiInstance.ThreadsUsersUsernameGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernameGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ThreadsUsersUsernameGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a Threads user profile by username
    ApiResponse<ThreadsUsersUsernameGet200Response> response = apiInstance.ThreadsUsersUsernameGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernameGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |

### Return type

[**ThreadsUsersUsernameGet200Response**](ThreadsUsersUsernameGet200Response.md)

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

<a id="threadsusersusernamepostsget"></a>
# **ThreadsUsersUsernamePostsGet**
> ThreadsSearchRecentGet200Response ThreadsUsersUsernamePostsGet (string username, string? cursor = null)

List Threads posts authored by a user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class ThreadsUsersUsernamePostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new ThreadsApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List Threads posts authored by a user
                ThreadsSearchRecentGet200Response result = apiInstance.ThreadsUsersUsernamePostsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernamePostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ThreadsUsersUsernamePostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Threads posts authored by a user
    ApiResponse<ThreadsSearchRecentGet200Response> response = apiInstance.ThreadsUsersUsernamePostsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernamePostsGetWithHttpInfo: " + e.Message);
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

[**ThreadsSearchRecentGet200Response**](ThreadsSearchRecentGet200Response.md)

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

<a id="threadsusersusernamerepliesget"></a>
# **ThreadsUsersUsernameRepliesGet**
> ThreadsSearchRecentGet200Response ThreadsUsersUsernameRepliesGet (string username, string? cursor = null)

List Threads replies authored by a user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class ThreadsUsersUsernameRepliesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new ThreadsApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List Threads replies authored by a user
                ThreadsSearchRecentGet200Response result = apiInstance.ThreadsUsersUsernameRepliesGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernameRepliesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ThreadsUsersUsernameRepliesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Threads replies authored by a user
    ApiResponse<ThreadsSearchRecentGet200Response> response = apiInstance.ThreadsUsersUsernameRepliesGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernameRepliesGetWithHttpInfo: " + e.Message);
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

[**ThreadsSearchRecentGet200Response**](ThreadsSearchRecentGet200Response.md)

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

<a id="threadsusersusernamerepostsget"></a>
# **ThreadsUsersUsernameRepostsGet**
> ThreadsSearchRecentGet200Response ThreadsUsersUsernameRepostsGet (string username, string? cursor = null)

List Threads reposts by a user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class ThreadsUsersUsernameRepostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new ThreadsApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List Threads reposts by a user
                ThreadsSearchRecentGet200Response result = apiInstance.ThreadsUsersUsernameRepostsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernameRepostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ThreadsUsersUsernameRepostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List Threads reposts by a user
    ApiResponse<ThreadsSearchRecentGet200Response> response = apiInstance.ThreadsUsersUsernameRepostsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling ThreadsApi.ThreadsUsersUsernameRepostsGetWithHttpInfo: " + e.Message);
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

[**ThreadsSearchRecentGet200Response**](ThreadsSearchRecentGet200Response.md)

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

