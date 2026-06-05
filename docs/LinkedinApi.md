# Unifapi.Sdk.Api.LinkedinApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**LinkedinAdsIdGet**](LinkedinApi.md#linkedinadsidget) | **GET** /linkedin/ads/{id} | Get a LinkedIn Ad Library entry by ID |
| [**LinkedinCompaniesSlugAffiliatedGet**](LinkedinApi.md#linkedincompaniesslugaffiliatedget) | **GET** /linkedin/companies/{slug}/affiliated | List a LinkedIn company&#39;s affiliated pages |
| [**LinkedinCompaniesSlugGet**](LinkedinApi.md#linkedincompaniesslugget) | **GET** /linkedin/companies/{slug} | Get a LinkedIn company profile by URL slug |
| [**LinkedinCompaniesSlugJobCountGet**](LinkedinApi.md#linkedincompaniesslugjobcountget) | **GET** /linkedin/companies/{slug}/job-count | Get the number of active jobs at a LinkedIn company |
| [**LinkedinCompaniesSlugJobsGet**](LinkedinApi.md#linkedincompaniesslugjobsget) | **GET** /linkedin/companies/{slug}/jobs | List active job postings at a LinkedIn company |
| [**LinkedinCompaniesSlugMemberInsightsGet**](LinkedinApi.md#linkedincompaniesslugmemberinsightsget) | **GET** /linkedin/companies/{slug}/member-insights | Get a LinkedIn company&#39;s aggregated member insights |
| [**LinkedinCompaniesSlugPeopleGet**](LinkedinApi.md#linkedincompaniesslugpeopleget) | **GET** /linkedin/companies/{slug}/people | List employees of a LinkedIn company |
| [**LinkedinCompaniesSlugPostsGet**](LinkedinApi.md#linkedincompaniesslugpostsget) | **GET** /linkedin/companies/{slug}/posts | List posts published by a LinkedIn company page |
| [**LinkedinGroupsIdGet**](LinkedinApi.md#linkedingroupsidget) | **GET** /linkedin/groups/{id} | Get a LinkedIn group by ID |
| [**LinkedinGroupsIdPostsGet**](LinkedinApi.md#linkedingroupsidpostsget) | **GET** /linkedin/groups/{id}/posts | List posts in a LinkedIn group |
| [**LinkedinJobsIdGet**](LinkedinApi.md#linkedinjobsidget) | **GET** /linkedin/jobs/{id} | Get a LinkedIn job posting by ID |
| [**LinkedinPostsIdCommentsCommentIdRepliesGet**](LinkedinApi.md#linkedinpostsidcommentscommentidrepliesget) | **GET** /linkedin/posts/{id}/comments/{comment_id}/replies | List replies to a LinkedIn comment |
| [**LinkedinPostsIdCommentsGet**](LinkedinApi.md#linkedinpostsidcommentsget) | **GET** /linkedin/posts/{id}/comments | List top-level comments on a LinkedIn post |
| [**LinkedinPostsIdGet**](LinkedinApi.md#linkedinpostsidget) | **GET** /linkedin/posts/{id} | Get a LinkedIn post by ID |
| [**LinkedinPostsIdReactionsGet**](LinkedinApi.md#linkedinpostsidreactionsget) | **GET** /linkedin/posts/{id}/reactions | List users who reacted to a LinkedIn post |
| [**LinkedinPostsIdRepostsGet**](LinkedinApi.md#linkedinpostsidrepostsget) | **GET** /linkedin/posts/{id}/reposts | List reposts of a LinkedIn post |
| [**LinkedinSearchAdsGet**](LinkedinApi.md#linkedinsearchadsget) | **GET** /linkedin/search/ads | Search the LinkedIn Ad Library |
| [**LinkedinSearchIndustriesGet**](LinkedinApi.md#linkedinsearchindustriesget) | **GET** /linkedin/search/industries | Resolve a free-text industry name to LinkedIn industry IDs |
| [**LinkedinSearchJobsGet**](LinkedinApi.md#linkedinsearchjobsget) | **GET** /linkedin/search/jobs | Search LinkedIn jobs by keyword and filters |
| [**LinkedinSearchLocationsGet**](LinkedinApi.md#linkedinsearchlocationsget) | **GET** /linkedin/search/locations | Resolve a free-text location into LinkedIn geocode tokens |
| [**LinkedinSearchPeopleGet**](LinkedinApi.md#linkedinsearchpeopleget) | **GET** /linkedin/search/people | Search LinkedIn people by name, title, company, etc. |
| [**LinkedinSearchPostsGet**](LinkedinApi.md#linkedinsearchpostsget) | **GET** /linkedin/search/posts | Search LinkedIn posts by keyword |
| [**LinkedinSearchSchoolsGet**](LinkedinApi.md#linkedinsearchschoolsget) | **GET** /linkedin/search/schools | Search LinkedIn schools by keyword |
| [**LinkedinUsersUsernameAboutGet**](LinkedinApi.md#linkedinusersusernameaboutget) | **GET** /linkedin/users/{username}/about | Get a LinkedIn profile&#39;s &#39;about&#39; metadata |
| [**LinkedinUsersUsernameCertificationsGet**](LinkedinApi.md#linkedinusersusernamecertificationsget) | **GET** /linkedin/users/{username}/certifications | List a LinkedIn user&#39;s certifications |
| [**LinkedinUsersUsernameCommentsGet**](LinkedinApi.md#linkedinusersusernamecommentsget) | **GET** /linkedin/users/{username}/comments | List comments authored by a LinkedIn user |
| [**LinkedinUsersUsernameContactGet**](LinkedinApi.md#linkedinusersusernamecontactget) | **GET** /linkedin/users/{username}/contact | Get a LinkedIn user&#39;s public contact info |
| [**LinkedinUsersUsernameEducationsGet**](LinkedinApi.md#linkedinusersusernameeducationsget) | **GET** /linkedin/users/{username}/educations | List a LinkedIn user&#39;s education |
| [**LinkedinUsersUsernameExperienceGet**](LinkedinApi.md#linkedinusersusernameexperienceget) | **GET** /linkedin/users/{username}/experience | List a LinkedIn user&#39;s work experience |
| [**LinkedinUsersUsernameFollowerCountGet**](LinkedinApi.md#linkedinusersusernamefollowercountget) | **GET** /linkedin/users/{username}/follower-count | Get a LinkedIn user&#39;s follower &amp; connection counts |
| [**LinkedinUsersUsernameGet**](LinkedinApi.md#linkedinusersusernameget) | **GET** /linkedin/users/{username} | Get a LinkedIn user profile by URL slug |
| [**LinkedinUsersUsernameHonorsGet**](LinkedinApi.md#linkedinusersusernamehonorsget) | **GET** /linkedin/users/{username}/honors | List a LinkedIn user&#39;s honors and awards |
| [**LinkedinUsersUsernameImagesGet**](LinkedinApi.md#linkedinusersusernameimagesget) | **GET** /linkedin/users/{username}/images | List image posts authored by a LinkedIn user |
| [**LinkedinUsersUsernameInterestsCompaniesGet**](LinkedinApi.md#linkedinusersusernameinterestscompaniesget) | **GET** /linkedin/users/{username}/interests/companies | List companies a LinkedIn user follows |
| [**LinkedinUsersUsernameInterestsGroupsGet**](LinkedinApi.md#linkedinusersusernameinterestsgroupsget) | **GET** /linkedin/users/{username}/interests/groups | List LinkedIn groups a user follows |
| [**LinkedinUsersUsernamePostsGet**](LinkedinApi.md#linkedinusersusernamepostsget) | **GET** /linkedin/users/{username}/posts | List posts authored by a LinkedIn user |
| [**LinkedinUsersUsernamePublicationsGet**](LinkedinApi.md#linkedinusersusernamepublicationsget) | **GET** /linkedin/users/{username}/publications | List a LinkedIn user&#39;s publications |
| [**LinkedinUsersUsernameReactionsGet**](LinkedinApi.md#linkedinusersusernamereactionsget) | **GET** /linkedin/users/{username}/reactions | List reactions a LinkedIn user has placed on posts |
| [**LinkedinUsersUsernameRecommendationsGet**](LinkedinApi.md#linkedinusersusernamerecommendationsget) | **GET** /linkedin/users/{username}/recommendations | List recommendations written for a LinkedIn user |
| [**LinkedinUsersUsernameSkillsGet**](LinkedinApi.md#linkedinusersusernameskillsget) | **GET** /linkedin/users/{username}/skills | List a LinkedIn user&#39;s skills |
| [**LinkedinUsersUsernameVideosGet**](LinkedinApi.md#linkedinusersusernamevideosget) | **GET** /linkedin/users/{username}/videos | List video posts authored by a LinkedIn user |
| [**LinkedinUsersUsernameVolunteersGet**](LinkedinApi.md#linkedinusersusernamevolunteersget) | **GET** /linkedin/users/{username}/volunteers | List a LinkedIn user&#39;s volunteer experience |

<a id="linkedinadsidget"></a>
# **LinkedinAdsIdGet**
> LinkedinAdsIdGet200Response LinkedinAdsIdGet (string id)

Get a LinkedIn Ad Library entry by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinAdsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 

            try
            {
                // Get a LinkedIn Ad Library entry by ID
                LinkedinAdsIdGet200Response result = apiInstance.LinkedinAdsIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinAdsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinAdsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn Ad Library entry by ID
    ApiResponse<LinkedinAdsIdGet200Response> response = apiInstance.LinkedinAdsIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinAdsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**LinkedinAdsIdGet200Response**](LinkedinAdsIdGet200Response.md)

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

<a id="linkedincompaniesslugaffiliatedget"></a>
# **LinkedinCompaniesSlugAffiliatedGet**
> LinkedinCompaniesSlugAffiliatedGet200Response LinkedinCompaniesSlugAffiliatedGet (string slug)

List a LinkedIn company's affiliated pages

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinCompaniesSlugAffiliatedGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var slug = "slug_example";  // string | 

            try
            {
                // List a LinkedIn company's affiliated pages
                LinkedinCompaniesSlugAffiliatedGet200Response result = apiInstance.LinkedinCompaniesSlugAffiliatedGet(slug);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugAffiliatedGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinCompaniesSlugAffiliatedGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn company's affiliated pages
    ApiResponse<LinkedinCompaniesSlugAffiliatedGet200Response> response = apiInstance.LinkedinCompaniesSlugAffiliatedGetWithHttpInfo(slug);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugAffiliatedGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **slug** | **string** |  |  |

### Return type

[**LinkedinCompaniesSlugAffiliatedGet200Response**](LinkedinCompaniesSlugAffiliatedGet200Response.md)

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

<a id="linkedincompaniesslugget"></a>
# **LinkedinCompaniesSlugGet**
> LinkedinCompaniesSlugGet200Response LinkedinCompaniesSlugGet (string slug)

Get a LinkedIn company profile by URL slug

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinCompaniesSlugGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var slug = "slug_example";  // string | LinkedIn URL slug (universal_name), e.g. `microsoft`

            try
            {
                // Get a LinkedIn company profile by URL slug
                LinkedinCompaniesSlugGet200Response result = apiInstance.LinkedinCompaniesSlugGet(slug);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinCompaniesSlugGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn company profile by URL slug
    ApiResponse<LinkedinCompaniesSlugGet200Response> response = apiInstance.LinkedinCompaniesSlugGetWithHttpInfo(slug);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **slug** | **string** | LinkedIn URL slug (universal_name), e.g. &#x60;microsoft&#x60; |  |

### Return type

[**LinkedinCompaniesSlugGet200Response**](LinkedinCompaniesSlugGet200Response.md)

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

<a id="linkedincompaniesslugjobcountget"></a>
# **LinkedinCompaniesSlugJobCountGet**
> LinkedinCompaniesSlugJobCountGet200Response LinkedinCompaniesSlugJobCountGet (string slug)

Get the number of active jobs at a LinkedIn company

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinCompaniesSlugJobCountGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var slug = "slug_example";  // string | 

            try
            {
                // Get the number of active jobs at a LinkedIn company
                LinkedinCompaniesSlugJobCountGet200Response result = apiInstance.LinkedinCompaniesSlugJobCountGet(slug);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugJobCountGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinCompaniesSlugJobCountGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get the number of active jobs at a LinkedIn company
    ApiResponse<LinkedinCompaniesSlugJobCountGet200Response> response = apiInstance.LinkedinCompaniesSlugJobCountGetWithHttpInfo(slug);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugJobCountGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **slug** | **string** |  |  |

### Return type

[**LinkedinCompaniesSlugJobCountGet200Response**](LinkedinCompaniesSlugJobCountGet200Response.md)

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

<a id="linkedincompaniesslugjobsget"></a>
# **LinkedinCompaniesSlugJobsGet**
> LinkedinCompaniesSlugJobsGet200Response LinkedinCompaniesSlugJobsGet (string slug, string? cursor = null)

List active job postings at a LinkedIn company

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinCompaniesSlugJobsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var slug = "slug_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List active job postings at a LinkedIn company
                LinkedinCompaniesSlugJobsGet200Response result = apiInstance.LinkedinCompaniesSlugJobsGet(slug, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugJobsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinCompaniesSlugJobsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List active job postings at a LinkedIn company
    ApiResponse<LinkedinCompaniesSlugJobsGet200Response> response = apiInstance.LinkedinCompaniesSlugJobsGetWithHttpInfo(slug, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugJobsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **slug** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**LinkedinCompaniesSlugJobsGet200Response**](LinkedinCompaniesSlugJobsGet200Response.md)

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

<a id="linkedincompaniesslugmemberinsightsget"></a>
# **LinkedinCompaniesSlugMemberInsightsGet**
> LinkedinCompaniesSlugMemberInsightsGet200Response LinkedinCompaniesSlugMemberInsightsGet (string slug)

Get a LinkedIn company's aggregated member insights

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinCompaniesSlugMemberInsightsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var slug = "slug_example";  // string | 

            try
            {
                // Get a LinkedIn company's aggregated member insights
                LinkedinCompaniesSlugMemberInsightsGet200Response result = apiInstance.LinkedinCompaniesSlugMemberInsightsGet(slug);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugMemberInsightsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinCompaniesSlugMemberInsightsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn company's aggregated member insights
    ApiResponse<LinkedinCompaniesSlugMemberInsightsGet200Response> response = apiInstance.LinkedinCompaniesSlugMemberInsightsGetWithHttpInfo(slug);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugMemberInsightsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **slug** | **string** |  |  |

### Return type

[**LinkedinCompaniesSlugMemberInsightsGet200Response**](LinkedinCompaniesSlugMemberInsightsGet200Response.md)

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

<a id="linkedincompaniesslugpeopleget"></a>
# **LinkedinCompaniesSlugPeopleGet**
> LinkedinCompaniesSlugPeopleGet200Response LinkedinCompaniesSlugPeopleGet (string slug, string? cursor = null)

List employees of a LinkedIn company

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinCompaniesSlugPeopleGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var slug = "slug_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List employees of a LinkedIn company
                LinkedinCompaniesSlugPeopleGet200Response result = apiInstance.LinkedinCompaniesSlugPeopleGet(slug, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugPeopleGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinCompaniesSlugPeopleGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List employees of a LinkedIn company
    ApiResponse<LinkedinCompaniesSlugPeopleGet200Response> response = apiInstance.LinkedinCompaniesSlugPeopleGetWithHttpInfo(slug, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugPeopleGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **slug** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**LinkedinCompaniesSlugPeopleGet200Response**](LinkedinCompaniesSlugPeopleGet200Response.md)

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

<a id="linkedincompaniesslugpostsget"></a>
# **LinkedinCompaniesSlugPostsGet**
> LinkedinCompaniesSlugPostsGet200Response LinkedinCompaniesSlugPostsGet (string slug, string? cursor = null)

List posts published by a LinkedIn company page

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinCompaniesSlugPostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var slug = "slug_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List posts published by a LinkedIn company page
                LinkedinCompaniesSlugPostsGet200Response result = apiInstance.LinkedinCompaniesSlugPostsGet(slug, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugPostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinCompaniesSlugPostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List posts published by a LinkedIn company page
    ApiResponse<LinkedinCompaniesSlugPostsGet200Response> response = apiInstance.LinkedinCompaniesSlugPostsGetWithHttpInfo(slug, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinCompaniesSlugPostsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **slug** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**LinkedinCompaniesSlugPostsGet200Response**](LinkedinCompaniesSlugPostsGet200Response.md)

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

<a id="linkedingroupsidget"></a>
# **LinkedinGroupsIdGet**
> LinkedinGroupsIdGet200Response LinkedinGroupsIdGet (string id)

Get a LinkedIn group by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinGroupsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 

            try
            {
                // Get a LinkedIn group by ID
                LinkedinGroupsIdGet200Response result = apiInstance.LinkedinGroupsIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinGroupsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinGroupsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn group by ID
    ApiResponse<LinkedinGroupsIdGet200Response> response = apiInstance.LinkedinGroupsIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinGroupsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**LinkedinGroupsIdGet200Response**](LinkedinGroupsIdGet200Response.md)

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

<a id="linkedingroupsidpostsget"></a>
# **LinkedinGroupsIdPostsGet**
> LinkedinCompaniesSlugPostsGet200Response LinkedinGroupsIdPostsGet (string id, string? cursor = null)

List posts in a LinkedIn group

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinGroupsIdPostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List posts in a LinkedIn group
                LinkedinCompaniesSlugPostsGet200Response result = apiInstance.LinkedinGroupsIdPostsGet(id, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinGroupsIdPostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinGroupsIdPostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List posts in a LinkedIn group
    ApiResponse<LinkedinCompaniesSlugPostsGet200Response> response = apiInstance.LinkedinGroupsIdPostsGetWithHttpInfo(id, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinGroupsIdPostsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**LinkedinCompaniesSlugPostsGet200Response**](LinkedinCompaniesSlugPostsGet200Response.md)

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

<a id="linkedinjobsidget"></a>
# **LinkedinJobsIdGet**
> LinkedinJobsIdGet200Response LinkedinJobsIdGet (string id, string? includeSkills = null)

Get a LinkedIn job posting by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinJobsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 
            var includeSkills = "true";  // string? |  (optional) 

            try
            {
                // Get a LinkedIn job posting by ID
                LinkedinJobsIdGet200Response result = apiInstance.LinkedinJobsIdGet(id, includeSkills);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinJobsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinJobsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn job posting by ID
    ApiResponse<LinkedinJobsIdGet200Response> response = apiInstance.LinkedinJobsIdGetWithHttpInfo(id, includeSkills);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinJobsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **includeSkills** | **string?** |  | [optional]  |

### Return type

[**LinkedinJobsIdGet200Response**](LinkedinJobsIdGet200Response.md)

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

<a id="linkedinpostsidcommentscommentidrepliesget"></a>
# **LinkedinPostsIdCommentsCommentIdRepliesGet**
> LinkedinPostsIdCommentsCommentIdRepliesGet200Response LinkedinPostsIdCommentsCommentIdRepliesGet (string id, string commentId, string? cursor = null)

List replies to a LinkedIn comment

`cursor` here is LinkedIn's `previous_replies_token`. On the first page, send no cursor — LinkedIn's source still expects the param, so the gateway passes `-` as the sentinel it documents.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinPostsIdCommentsCommentIdRepliesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 
            var commentId = "commentId_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List replies to a LinkedIn comment
                LinkedinPostsIdCommentsCommentIdRepliesGet200Response result = apiInstance.LinkedinPostsIdCommentsCommentIdRepliesGet(id, commentId, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdCommentsCommentIdRepliesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinPostsIdCommentsCommentIdRepliesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List replies to a LinkedIn comment
    ApiResponse<LinkedinPostsIdCommentsCommentIdRepliesGet200Response> response = apiInstance.LinkedinPostsIdCommentsCommentIdRepliesGetWithHttpInfo(id, commentId, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdCommentsCommentIdRepliesGetWithHttpInfo: " + e.Message);
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

### Return type

[**LinkedinPostsIdCommentsCommentIdRepliesGet200Response**](LinkedinPostsIdCommentsCommentIdRepliesGet200Response.md)

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

<a id="linkedinpostsidcommentsget"></a>
# **LinkedinPostsIdCommentsGet**
> LinkedinPostsIdCommentsCommentIdRepliesGet200Response LinkedinPostsIdCommentsGet (string id, string? cursor = null)

List top-level comments on a LinkedIn post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinPostsIdCommentsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List top-level comments on a LinkedIn post
                LinkedinPostsIdCommentsCommentIdRepliesGet200Response result = apiInstance.LinkedinPostsIdCommentsGet(id, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdCommentsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinPostsIdCommentsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List top-level comments on a LinkedIn post
    ApiResponse<LinkedinPostsIdCommentsCommentIdRepliesGet200Response> response = apiInstance.LinkedinPostsIdCommentsGetWithHttpInfo(id, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdCommentsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**LinkedinPostsIdCommentsCommentIdRepliesGet200Response**](LinkedinPostsIdCommentsCommentIdRepliesGet200Response.md)

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

<a id="linkedinpostsidget"></a>
# **LinkedinPostsIdGet**
> LinkedinPostsIdGet200Response LinkedinPostsIdGet (string id)

Get a LinkedIn post by ID

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinPostsIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 

            try
            {
                // Get a LinkedIn post by ID
                LinkedinPostsIdGet200Response result = apiInstance.LinkedinPostsIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinPostsIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn post by ID
    ApiResponse<LinkedinPostsIdGet200Response> response = apiInstance.LinkedinPostsIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |

### Return type

[**LinkedinPostsIdGet200Response**](LinkedinPostsIdGet200Response.md)

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

<a id="linkedinpostsidreactionsget"></a>
# **LinkedinPostsIdReactionsGet**
> LinkedinCompaniesSlugPeopleGet200Response LinkedinPostsIdReactionsGet (string id, string? cursor = null, string? type = null)

List users who reacted to a LinkedIn post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinPostsIdReactionsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var type = "all";  // string? | Filter by reaction type. `all` returns every reaction (default). (optional)  (default to all)

            try
            {
                // List users who reacted to a LinkedIn post
                LinkedinCompaniesSlugPeopleGet200Response result = apiInstance.LinkedinPostsIdReactionsGet(id, cursor, type);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdReactionsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinPostsIdReactionsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List users who reacted to a LinkedIn post
    ApiResponse<LinkedinCompaniesSlugPeopleGet200Response> response = apiInstance.LinkedinPostsIdReactionsGetWithHttpInfo(id, cursor, type);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdReactionsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **type** | **string?** | Filter by reaction type. &#x60;all&#x60; returns every reaction (default). | [optional] [default to all] |

### Return type

[**LinkedinCompaniesSlugPeopleGet200Response**](LinkedinCompaniesSlugPeopleGet200Response.md)

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

<a id="linkedinpostsidrepostsget"></a>
# **LinkedinPostsIdRepostsGet**
> LinkedinCompaniesSlugPostsGet200Response LinkedinPostsIdRepostsGet (string id, string? cursor = null)

List reposts of a LinkedIn post

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinPostsIdRepostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var id = "id_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List reposts of a LinkedIn post
                LinkedinCompaniesSlugPostsGet200Response result = apiInstance.LinkedinPostsIdRepostsGet(id, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdRepostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinPostsIdRepostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List reposts of a LinkedIn post
    ApiResponse<LinkedinCompaniesSlugPostsGet200Response> response = apiInstance.LinkedinPostsIdRepostsGetWithHttpInfo(id, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinPostsIdRepostsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**LinkedinCompaniesSlugPostsGet200Response**](LinkedinCompaniesSlugPostsGet200Response.md)

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

<a id="linkedinsearchadsget"></a>
# **LinkedinSearchAdsGet**
> LinkedinSearchAdsGet200Response LinkedinSearchAdsGet (string? cursor = null, string? keyword = null, string? advertiserName = null, string? country = null, string? date = null)

Search the LinkedIn Ad Library

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinSearchAdsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var cursor = "cursor_example";  // string? |  (optional) 
            var keyword = "keyword_example";  // string? |  (optional) 
            var advertiserName = "advertiserName_example";  // string? |  (optional) 
            var country = "country_example";  // string? | ISO-3166-1 alpha-2 code, e.g. `US` (optional) 
            var date = "date_example";  // string? |  (optional) 

            try
            {
                // Search the LinkedIn Ad Library
                LinkedinSearchAdsGet200Response result = apiInstance.LinkedinSearchAdsGet(cursor, keyword, advertiserName, country, date);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinSearchAdsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinSearchAdsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search the LinkedIn Ad Library
    ApiResponse<LinkedinSearchAdsGet200Response> response = apiInstance.LinkedinSearchAdsGetWithHttpInfo(cursor, keyword, advertiserName, country, date);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinSearchAdsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **cursor** | **string?** |  | [optional]  |
| **keyword** | **string?** |  | [optional]  |
| **advertiserName** | **string?** |  | [optional]  |
| **country** | **string?** | ISO-3166-1 alpha-2 code, e.g. &#x60;US&#x60; | [optional]  |
| **date** | **string?** |  | [optional]  |

### Return type

[**LinkedinSearchAdsGet200Response**](LinkedinSearchAdsGet200Response.md)

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

<a id="linkedinsearchindustriesget"></a>
# **LinkedinSearchIndustriesGet**
> LinkedinSearchIndustriesGet200Response LinkedinSearchIndustriesGet (string keyword)

Resolve a free-text industry name to LinkedIn industry IDs

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinSearchIndustriesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var keyword = "keyword_example";  // string | 

            try
            {
                // Resolve a free-text industry name to LinkedIn industry IDs
                LinkedinSearchIndustriesGet200Response result = apiInstance.LinkedinSearchIndustriesGet(keyword);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinSearchIndustriesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinSearchIndustriesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Resolve a free-text industry name to LinkedIn industry IDs
    ApiResponse<LinkedinSearchIndustriesGet200Response> response = apiInstance.LinkedinSearchIndustriesGetWithHttpInfo(keyword);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinSearchIndustriesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **keyword** | **string** |  |  |

### Return type

[**LinkedinSearchIndustriesGet200Response**](LinkedinSearchIndustriesGet200Response.md)

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

<a id="linkedinsearchjobsget"></a>
# **LinkedinSearchJobsGet**
> LinkedinCompaniesSlugJobsGet200Response LinkedinSearchJobsGet (string keyword, string? cursor = null, string? sortBy = null, string? datePosted = null, string? geocode = null, string? company = null, string? experienceLevel = null, string? remote = null, string? jobType = null, string? easyApply = null, string? hasVerifications = null, string? under10Applicants = null, string? fairChanceEmployer = null)

Search LinkedIn jobs by keyword and filters

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinSearchJobsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var keyword = "keyword_example";  // string | Free-text search query
            var cursor = "cursor_example";  // string? |  (optional) 
            var sortBy = "sortBy_example";  // string? |  (optional) 
            var datePosted = "datePosted_example";  // string? |  (optional) 
            var geocode = "geocode_example";  // string? |  (optional) 
            var company = "company_example";  // string? |  (optional) 
            var experienceLevel = "experienceLevel_example";  // string? |  (optional) 
            var remote = "remote_example";  // string? |  (optional) 
            var jobType = "jobType_example";  // string? |  (optional) 
            var easyApply = "true";  // string? |  (optional) 
            var hasVerifications = "true";  // string? |  (optional) 
            var under10Applicants = "true";  // string? |  (optional) 
            var fairChanceEmployer = "true";  // string? |  (optional) 

            try
            {
                // Search LinkedIn jobs by keyword and filters
                LinkedinCompaniesSlugJobsGet200Response result = apiInstance.LinkedinSearchJobsGet(keyword, cursor, sortBy, datePosted, geocode, company, experienceLevel, remote, jobType, easyApply, hasVerifications, under10Applicants, fairChanceEmployer);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinSearchJobsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinSearchJobsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search LinkedIn jobs by keyword and filters
    ApiResponse<LinkedinCompaniesSlugJobsGet200Response> response = apiInstance.LinkedinSearchJobsGetWithHttpInfo(keyword, cursor, sortBy, datePosted, geocode, company, experienceLevel, remote, jobType, easyApply, hasVerifications, under10Applicants, fairChanceEmployer);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinSearchJobsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **keyword** | **string** | Free-text search query |  |
| **cursor** | **string?** |  | [optional]  |
| **sortBy** | **string?** |  | [optional]  |
| **datePosted** | **string?** |  | [optional]  |
| **geocode** | **string?** |  | [optional]  |
| **company** | **string?** |  | [optional]  |
| **experienceLevel** | **string?** |  | [optional]  |
| **remote** | **string?** |  | [optional]  |
| **jobType** | **string?** |  | [optional]  |
| **easyApply** | **string?** |  | [optional]  |
| **hasVerifications** | **string?** |  | [optional]  |
| **under10Applicants** | **string?** |  | [optional]  |
| **fairChanceEmployer** | **string?** |  | [optional]  |

### Return type

[**LinkedinCompaniesSlugJobsGet200Response**](LinkedinCompaniesSlugJobsGet200Response.md)

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

<a id="linkedinsearchlocationsget"></a>
# **LinkedinSearchLocationsGet**
> LinkedinSearchLocationsGet200Response LinkedinSearchLocationsGet (string keyword)

Resolve a free-text location into LinkedIn geocode tokens

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinSearchLocationsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var keyword = "keyword_example";  // string | 

            try
            {
                // Resolve a free-text location into LinkedIn geocode tokens
                LinkedinSearchLocationsGet200Response result = apiInstance.LinkedinSearchLocationsGet(keyword);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinSearchLocationsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinSearchLocationsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Resolve a free-text location into LinkedIn geocode tokens
    ApiResponse<LinkedinSearchLocationsGet200Response> response = apiInstance.LinkedinSearchLocationsGetWithHttpInfo(keyword);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinSearchLocationsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **keyword** | **string** |  |  |

### Return type

[**LinkedinSearchLocationsGet200Response**](LinkedinSearchLocationsGet200Response.md)

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

<a id="linkedinsearchpeopleget"></a>
# **LinkedinSearchPeopleGet**
> LinkedinCompaniesSlugPeopleGet200Response LinkedinSearchPeopleGet (string? cursor = null, string? name = null, string? firstName = null, string? lastName = null, string? title = null, string? company = null, string? school = null, string? geocodeLocation = null, string? currentCompany = null, string? profileLanguage = null, string? industry = null, string? serviceCategory = null)

Search LinkedIn people by name, title, company, etc.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinSearchPeopleGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var cursor = "cursor_example";  // string? |  (optional) 
            var name = "name_example";  // string? |  (optional) 
            var firstName = "firstName_example";  // string? |  (optional) 
            var lastName = "lastName_example";  // string? |  (optional) 
            var title = "title_example";  // string? |  (optional) 
            var company = "company_example";  // string? |  (optional) 
            var school = "school_example";  // string? |  (optional) 
            var geocodeLocation = "geocodeLocation_example";  // string? |  (optional) 
            var currentCompany = "currentCompany_example";  // string? |  (optional) 
            var profileLanguage = "profileLanguage_example";  // string? |  (optional) 
            var industry = "industry_example";  // string? |  (optional) 
            var serviceCategory = "serviceCategory_example";  // string? |  (optional) 

            try
            {
                // Search LinkedIn people by name, title, company, etc.
                LinkedinCompaniesSlugPeopleGet200Response result = apiInstance.LinkedinSearchPeopleGet(cursor, name, firstName, lastName, title, company, school, geocodeLocation, currentCompany, profileLanguage, industry, serviceCategory);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinSearchPeopleGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinSearchPeopleGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search LinkedIn people by name, title, company, etc.
    ApiResponse<LinkedinCompaniesSlugPeopleGet200Response> response = apiInstance.LinkedinSearchPeopleGetWithHttpInfo(cursor, name, firstName, lastName, title, company, school, geocodeLocation, currentCompany, profileLanguage, industry, serviceCategory);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinSearchPeopleGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **cursor** | **string?** |  | [optional]  |
| **name** | **string?** |  | [optional]  |
| **firstName** | **string?** |  | [optional]  |
| **lastName** | **string?** |  | [optional]  |
| **title** | **string?** |  | [optional]  |
| **company** | **string?** |  | [optional]  |
| **school** | **string?** |  | [optional]  |
| **geocodeLocation** | **string?** |  | [optional]  |
| **currentCompany** | **string?** |  | [optional]  |
| **profileLanguage** | **string?** |  | [optional]  |
| **industry** | **string?** |  | [optional]  |
| **serviceCategory** | **string?** |  | [optional]  |

### Return type

[**LinkedinCompaniesSlugPeopleGet200Response**](LinkedinCompaniesSlugPeopleGet200Response.md)

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

<a id="linkedinsearchpostsget"></a>
# **LinkedinSearchPostsGet**
> LinkedinSearchPostsGet200Response LinkedinSearchPostsGet (string keyword, string? cursor = null, string? datePosted = null, string? sortBy = null, string? fromMember = null, string? fromCompany = null, string? contentType = null)

Search LinkedIn posts by keyword

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinSearchPostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var keyword = "keyword_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 
            var datePosted = "datePosted_example";  // string? |  (optional) 
            var sortBy = "sortBy_example";  // string? |  (optional) 
            var fromMember = "fromMember_example";  // string? |  (optional) 
            var fromCompany = "fromCompany_example";  // string? |  (optional) 
            var contentType = "contentType_example";  // string? |  (optional) 

            try
            {
                // Search LinkedIn posts by keyword
                LinkedinSearchPostsGet200Response result = apiInstance.LinkedinSearchPostsGet(keyword, cursor, datePosted, sortBy, fromMember, fromCompany, contentType);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinSearchPostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinSearchPostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search LinkedIn posts by keyword
    ApiResponse<LinkedinSearchPostsGet200Response> response = apiInstance.LinkedinSearchPostsGetWithHttpInfo(keyword, cursor, datePosted, sortBy, fromMember, fromCompany, contentType);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinSearchPostsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **keyword** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |
| **datePosted** | **string?** |  | [optional]  |
| **sortBy** | **string?** |  | [optional]  |
| **fromMember** | **string?** |  | [optional]  |
| **fromCompany** | **string?** |  | [optional]  |
| **contentType** | **string?** |  | [optional]  |

### Return type

[**LinkedinSearchPostsGet200Response**](LinkedinSearchPostsGet200Response.md)

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

<a id="linkedinsearchschoolsget"></a>
# **LinkedinSearchSchoolsGet**
> LinkedinSearchSchoolsGet200Response LinkedinSearchSchoolsGet (string keyword, string? cursor = null)

Search LinkedIn schools by keyword

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinSearchSchoolsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var keyword = "keyword_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // Search LinkedIn schools by keyword
                LinkedinSearchSchoolsGet200Response result = apiInstance.LinkedinSearchSchoolsGet(keyword, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinSearchSchoolsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinSearchSchoolsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Search LinkedIn schools by keyword
    ApiResponse<LinkedinSearchSchoolsGet200Response> response = apiInstance.LinkedinSearchSchoolsGetWithHttpInfo(keyword, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinSearchSchoolsGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **keyword** | **string** |  |  |
| **cursor** | **string?** |  | [optional]  |

### Return type

[**LinkedinSearchSchoolsGet200Response**](LinkedinSearchSchoolsGet200Response.md)

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

<a id="linkedinusersusernameaboutget"></a>
# **LinkedinUsersUsernameAboutGet**
> LinkedinUsersUsernameAboutGet200Response LinkedinUsersUsernameAboutGet (string username)

Get a LinkedIn profile's 'about' metadata

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameAboutGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 

            try
            {
                // Get a LinkedIn profile's 'about' metadata
                LinkedinUsersUsernameAboutGet200Response result = apiInstance.LinkedinUsersUsernameAboutGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameAboutGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameAboutGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn profile's 'about' metadata
    ApiResponse<LinkedinUsersUsernameAboutGet200Response> response = apiInstance.LinkedinUsersUsernameAboutGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameAboutGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |

### Return type

[**LinkedinUsersUsernameAboutGet200Response**](LinkedinUsersUsernameAboutGet200Response.md)

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

<a id="linkedinusersusernamecertificationsget"></a>
# **LinkedinUsersUsernameCertificationsGet**
> LinkedinUsersUsernameCertificationsGet200Response LinkedinUsersUsernameCertificationsGet (string username, string? cursor = null)

List a LinkedIn user's certifications

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameCertificationsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List a LinkedIn user's certifications
                LinkedinUsersUsernameCertificationsGet200Response result = apiInstance.LinkedinUsersUsernameCertificationsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameCertificationsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameCertificationsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn user's certifications
    ApiResponse<LinkedinUsersUsernameCertificationsGet200Response> response = apiInstance.LinkedinUsersUsernameCertificationsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameCertificationsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameCertificationsGet200Response**](LinkedinUsersUsernameCertificationsGet200Response.md)

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

<a id="linkedinusersusernamecommentsget"></a>
# **LinkedinUsersUsernameCommentsGet**
> LinkedinUsersUsernameCommentsGet200Response LinkedinUsersUsernameCommentsGet (string username, string? cursor = null)

List comments authored by a LinkedIn user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameCommentsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List comments authored by a LinkedIn user
                LinkedinUsersUsernameCommentsGet200Response result = apiInstance.LinkedinUsersUsernameCommentsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameCommentsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameCommentsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List comments authored by a LinkedIn user
    ApiResponse<LinkedinUsersUsernameCommentsGet200Response> response = apiInstance.LinkedinUsersUsernameCommentsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameCommentsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameCommentsGet200Response**](LinkedinUsersUsernameCommentsGet200Response.md)

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

<a id="linkedinusersusernamecontactget"></a>
# **LinkedinUsersUsernameContactGet**
> LinkedinUsersUsernameContactGet200Response LinkedinUsersUsernameContactGet (string username)

Get a LinkedIn user's public contact info

Returns the contact block (websites, phone numbers, twitter handles, address, wechat) the user has chosen to publish on LinkedIn.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameContactGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 

            try
            {
                // Get a LinkedIn user's public contact info
                LinkedinUsersUsernameContactGet200Response result = apiInstance.LinkedinUsersUsernameContactGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameContactGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameContactGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn user's public contact info
    ApiResponse<LinkedinUsersUsernameContactGet200Response> response = apiInstance.LinkedinUsersUsernameContactGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameContactGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |

### Return type

[**LinkedinUsersUsernameContactGet200Response**](LinkedinUsersUsernameContactGet200Response.md)

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

<a id="linkedinusersusernameeducationsget"></a>
# **LinkedinUsersUsernameEducationsGet**
> LinkedinUsersUsernameEducationsGet200Response LinkedinUsersUsernameEducationsGet (string username, string? cursor = null)

List a LinkedIn user's education

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameEducationsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List a LinkedIn user's education
                LinkedinUsersUsernameEducationsGet200Response result = apiInstance.LinkedinUsersUsernameEducationsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameEducationsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameEducationsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn user's education
    ApiResponse<LinkedinUsersUsernameEducationsGet200Response> response = apiInstance.LinkedinUsersUsernameEducationsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameEducationsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameEducationsGet200Response**](LinkedinUsersUsernameEducationsGet200Response.md)

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

<a id="linkedinusersusernameexperienceget"></a>
# **LinkedinUsersUsernameExperienceGet**
> LinkedinUsersUsernameExperienceGet200Response LinkedinUsersUsernameExperienceGet (string username, string? cursor = null)

List a LinkedIn user's work experience

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameExperienceGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List a LinkedIn user's work experience
                LinkedinUsersUsernameExperienceGet200Response result = apiInstance.LinkedinUsersUsernameExperienceGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameExperienceGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameExperienceGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn user's work experience
    ApiResponse<LinkedinUsersUsernameExperienceGet200Response> response = apiInstance.LinkedinUsersUsernameExperienceGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameExperienceGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameExperienceGet200Response**](LinkedinUsersUsernameExperienceGet200Response.md)

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

<a id="linkedinusersusernamefollowercountget"></a>
# **LinkedinUsersUsernameFollowerCountGet**
> LinkedinUsersUsernameFollowerCountGet200Response LinkedinUsersUsernameFollowerCountGet (string username)

Get a LinkedIn user's follower & connection counts

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameFollowerCountGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 

            try
            {
                // Get a LinkedIn user's follower & connection counts
                LinkedinUsersUsernameFollowerCountGet200Response result = apiInstance.LinkedinUsersUsernameFollowerCountGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameFollowerCountGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameFollowerCountGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn user's follower & connection counts
    ApiResponse<LinkedinUsersUsernameFollowerCountGet200Response> response = apiInstance.LinkedinUsersUsernameFollowerCountGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameFollowerCountGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** |  |  |

### Return type

[**LinkedinUsersUsernameFollowerCountGet200Response**](LinkedinUsersUsernameFollowerCountGet200Response.md)

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

<a id="linkedinusersusernameget"></a>
# **LinkedinUsersUsernameGet**
> LinkedinUsersUsernameGet200Response LinkedinUsersUsernameGet (string username)

Get a LinkedIn user profile by URL slug

Returns the canonical LinkedIn profile for the given URL slug (`public_identifier`). Returns 404 not_found if no such user exists.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | LinkedIn URL slug, e.g. `williamhgates`

            try
            {
                // Get a LinkedIn user profile by URL slug
                LinkedinUsersUsernameGet200Response result = apiInstance.LinkedinUsersUsernameGet(username);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a LinkedIn user profile by URL slug
    ApiResponse<LinkedinUsersUsernameGet200Response> response = apiInstance.LinkedinUsersUsernameGetWithHttpInfo(username);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **username** | **string** | LinkedIn URL slug, e.g. &#x60;williamhgates&#x60; |  |

### Return type

[**LinkedinUsersUsernameGet200Response**](LinkedinUsersUsernameGet200Response.md)

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

<a id="linkedinusersusernamehonorsget"></a>
# **LinkedinUsersUsernameHonorsGet**
> LinkedinUsersUsernameHonorsGet200Response LinkedinUsersUsernameHonorsGet (string username, string? cursor = null)

List a LinkedIn user's honors and awards

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameHonorsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List a LinkedIn user's honors and awards
                LinkedinUsersUsernameHonorsGet200Response result = apiInstance.LinkedinUsersUsernameHonorsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameHonorsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameHonorsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn user's honors and awards
    ApiResponse<LinkedinUsersUsernameHonorsGet200Response> response = apiInstance.LinkedinUsersUsernameHonorsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameHonorsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameHonorsGet200Response**](LinkedinUsersUsernameHonorsGet200Response.md)

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

<a id="linkedinusersusernameimagesget"></a>
# **LinkedinUsersUsernameImagesGet**
> LinkedinUsersUsernameImagesGet200Response LinkedinUsersUsernameImagesGet (string username, string? cursor = null)

List image posts authored by a LinkedIn user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameImagesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List image posts authored by a LinkedIn user
                LinkedinUsersUsernameImagesGet200Response result = apiInstance.LinkedinUsersUsernameImagesGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameImagesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameImagesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List image posts authored by a LinkedIn user
    ApiResponse<LinkedinUsersUsernameImagesGet200Response> response = apiInstance.LinkedinUsersUsernameImagesGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameImagesGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameImagesGet200Response**](LinkedinUsersUsernameImagesGet200Response.md)

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

<a id="linkedinusersusernameinterestscompaniesget"></a>
# **LinkedinUsersUsernameInterestsCompaniesGet**
> LinkedinUsersUsernameInterestsCompaniesGet200Response LinkedinUsersUsernameInterestsCompaniesGet (string username, string? cursor = null)

List companies a LinkedIn user follows

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameInterestsCompaniesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List companies a LinkedIn user follows
                LinkedinUsersUsernameInterestsCompaniesGet200Response result = apiInstance.LinkedinUsersUsernameInterestsCompaniesGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameInterestsCompaniesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameInterestsCompaniesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List companies a LinkedIn user follows
    ApiResponse<LinkedinUsersUsernameInterestsCompaniesGet200Response> response = apiInstance.LinkedinUsersUsernameInterestsCompaniesGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameInterestsCompaniesGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameInterestsCompaniesGet200Response**](LinkedinUsersUsernameInterestsCompaniesGet200Response.md)

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

<a id="linkedinusersusernameinterestsgroupsget"></a>
# **LinkedinUsersUsernameInterestsGroupsGet**
> LinkedinUsersUsernameInterestsGroupsGet200Response LinkedinUsersUsernameInterestsGroupsGet (string username, string? cursor = null)

List LinkedIn groups a user follows

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameInterestsGroupsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List LinkedIn groups a user follows
                LinkedinUsersUsernameInterestsGroupsGet200Response result = apiInstance.LinkedinUsersUsernameInterestsGroupsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameInterestsGroupsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameInterestsGroupsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List LinkedIn groups a user follows
    ApiResponse<LinkedinUsersUsernameInterestsGroupsGet200Response> response = apiInstance.LinkedinUsersUsernameInterestsGroupsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameInterestsGroupsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameInterestsGroupsGet200Response**](LinkedinUsersUsernameInterestsGroupsGet200Response.md)

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

<a id="linkedinusersusernamepostsget"></a>
# **LinkedinUsersUsernamePostsGet**
> LinkedinCompaniesSlugPostsGet200Response LinkedinUsersUsernamePostsGet (string username, string? cursor = null)

List posts authored by a LinkedIn user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernamePostsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List posts authored by a LinkedIn user
                LinkedinCompaniesSlugPostsGet200Response result = apiInstance.LinkedinUsersUsernamePostsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernamePostsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernamePostsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List posts authored by a LinkedIn user
    ApiResponse<LinkedinCompaniesSlugPostsGet200Response> response = apiInstance.LinkedinUsersUsernamePostsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernamePostsGetWithHttpInfo: " + e.Message);
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

[**LinkedinCompaniesSlugPostsGet200Response**](LinkedinCompaniesSlugPostsGet200Response.md)

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

<a id="linkedinusersusernamepublicationsget"></a>
# **LinkedinUsersUsernamePublicationsGet**
> LinkedinUsersUsernamePublicationsGet200Response LinkedinUsersUsernamePublicationsGet (string username, string? cursor = null)

List a LinkedIn user's publications

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernamePublicationsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List a LinkedIn user's publications
                LinkedinUsersUsernamePublicationsGet200Response result = apiInstance.LinkedinUsersUsernamePublicationsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernamePublicationsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernamePublicationsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn user's publications
    ApiResponse<LinkedinUsersUsernamePublicationsGet200Response> response = apiInstance.LinkedinUsersUsernamePublicationsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernamePublicationsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernamePublicationsGet200Response**](LinkedinUsersUsernamePublicationsGet200Response.md)

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

<a id="linkedinusersusernamereactionsget"></a>
# **LinkedinUsersUsernameReactionsGet**
> LinkedinUsersUsernameReactionsGet200Response LinkedinUsersUsernameReactionsGet (string username, string? cursor = null)

List reactions a LinkedIn user has placed on posts

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameReactionsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List reactions a LinkedIn user has placed on posts
                LinkedinUsersUsernameReactionsGet200Response result = apiInstance.LinkedinUsersUsernameReactionsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameReactionsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameReactionsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List reactions a LinkedIn user has placed on posts
    ApiResponse<LinkedinUsersUsernameReactionsGet200Response> response = apiInstance.LinkedinUsersUsernameReactionsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameReactionsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameReactionsGet200Response**](LinkedinUsersUsernameReactionsGet200Response.md)

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

<a id="linkedinusersusernamerecommendationsget"></a>
# **LinkedinUsersUsernameRecommendationsGet**
> LinkedinUsersUsernameRecommendationsGet200Response LinkedinUsersUsernameRecommendationsGet (string username, string? cursor = null)

List recommendations written for a LinkedIn user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameRecommendationsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List recommendations written for a LinkedIn user
                LinkedinUsersUsernameRecommendationsGet200Response result = apiInstance.LinkedinUsersUsernameRecommendationsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameRecommendationsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameRecommendationsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List recommendations written for a LinkedIn user
    ApiResponse<LinkedinUsersUsernameRecommendationsGet200Response> response = apiInstance.LinkedinUsersUsernameRecommendationsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameRecommendationsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameRecommendationsGet200Response**](LinkedinUsersUsernameRecommendationsGet200Response.md)

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

<a id="linkedinusersusernameskillsget"></a>
# **LinkedinUsersUsernameSkillsGet**
> LinkedinUsersUsernameSkillsGet200Response LinkedinUsersUsernameSkillsGet (string username, string? cursor = null)

List a LinkedIn user's skills

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameSkillsGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List a LinkedIn user's skills
                LinkedinUsersUsernameSkillsGet200Response result = apiInstance.LinkedinUsersUsernameSkillsGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameSkillsGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameSkillsGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn user's skills
    ApiResponse<LinkedinUsersUsernameSkillsGet200Response> response = apiInstance.LinkedinUsersUsernameSkillsGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameSkillsGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameSkillsGet200Response**](LinkedinUsersUsernameSkillsGet200Response.md)

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

<a id="linkedinusersusernamevideosget"></a>
# **LinkedinUsersUsernameVideosGet**
> LinkedinUsersUsernameVideosGet200Response LinkedinUsersUsernameVideosGet (string username, string? cursor = null)

List video posts authored by a LinkedIn user

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameVideosGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List video posts authored by a LinkedIn user
                LinkedinUsersUsernameVideosGet200Response result = apiInstance.LinkedinUsersUsernameVideosGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameVideosGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameVideosGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List video posts authored by a LinkedIn user
    ApiResponse<LinkedinUsersUsernameVideosGet200Response> response = apiInstance.LinkedinUsersUsernameVideosGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameVideosGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameVideosGet200Response**](LinkedinUsersUsernameVideosGet200Response.md)

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

<a id="linkedinusersusernamevolunteersget"></a>
# **LinkedinUsersUsernameVolunteersGet**
> LinkedinUsersUsernameVolunteersGet200Response LinkedinUsersUsernameVolunteersGet (string username, string? cursor = null)

List a LinkedIn user's volunteer experience

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class LinkedinUsersUsernameVolunteersGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new LinkedinApi(config);
            var username = "username_example";  // string | 
            var cursor = "cursor_example";  // string? |  (optional) 

            try
            {
                // List a LinkedIn user's volunteer experience
                LinkedinUsersUsernameVolunteersGet200Response result = apiInstance.LinkedinUsersUsernameVolunteersGet(username, cursor);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameVolunteersGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the LinkedinUsersUsernameVolunteersGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a LinkedIn user's volunteer experience
    ApiResponse<LinkedinUsersUsernameVolunteersGet200Response> response = apiInstance.LinkedinUsersUsernameVolunteersGetWithHttpInfo(username, cursor);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling LinkedinApi.LinkedinUsersUsernameVolunteersGetWithHttpInfo: " + e.Message);
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

[**LinkedinUsersUsernameVolunteersGet200Response**](LinkedinUsersUsernameVolunteersGet200Response.md)

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

