# Unifapi.Sdk.Api.SeoApi

All URIs are relative to *https://api.unifapi.com*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**SeoBacklinksAnchorsPost**](SeoApi.md#seobacklinksanchorspost) | **POST** /seo/backlinks/anchors | Get anchor texts used in backlinks to a target |
| [**SeoBacklinksBulkBacklinksPost**](SeoApi.md#seobacklinksbulkbacklinkspost) | **POST** /seo/backlinks/bulk-backlinks | Count backlinks for many targets |
| [**SeoBacklinksBulkNewLostBacklinksPost**](SeoApi.md#seobacklinksbulknewlostbacklinkspost) | **POST** /seo/backlinks/bulk-new-lost-backlinks | Count new and lost backlinks for many targets |
| [**SeoBacklinksBulkNewLostReferringDomainsPost**](SeoApi.md#seobacklinksbulknewlostreferringdomainspost) | **POST** /seo/backlinks/bulk-new-lost-referring-domains | Count new and lost referring domains for many targets |
| [**SeoBacklinksBulkPagesSummaryPost**](SeoApi.md#seobacklinksbulkpagessummarypost) | **POST** /seo/backlinks/bulk-pages-summary | Summarize backlinks for many pages at once |
| [**SeoBacklinksBulkRanksPost**](SeoApi.md#seobacklinksbulkrankspost) | **POST** /seo/backlinks/bulk-ranks | Get backlink ranks for many targets |
| [**SeoBacklinksBulkReferringDomainsPost**](SeoApi.md#seobacklinksbulkreferringdomainspost) | **POST** /seo/backlinks/bulk-referring-domains | Count referring domains for many targets |
| [**SeoBacklinksBulkSpamScorePost**](SeoApi.md#seobacklinksbulkspamscorepost) | **POST** /seo/backlinks/bulk-spam-score | Get spam scores for many targets |
| [**SeoBacklinksCompetitorsPost**](SeoApi.md#seobacklinkscompetitorspost) | **POST** /seo/backlinks/competitors | Find competitors by shared referring domains |
| [**SeoBacklinksDomainIntersectionPost**](SeoApi.md#seobacklinksdomainintersectionpost) | **POST** /seo/backlinks/domain-intersection | Find domains linking to multiple targets |
| [**SeoBacklinksDomainPagesPost**](SeoApi.md#seobacklinksdomainpagespost) | **POST** /seo/backlinks/domain-pages | List target pages ranked by backlinks |
| [**SeoBacklinksDomainPagesSummaryPost**](SeoApi.md#seobacklinksdomainpagessummarypost) | **POST** /seo/backlinks/domain-pages-summary | Summarize backlinks for each page of a target |
| [**SeoBacklinksHistoryPost**](SeoApi.md#seobacklinkshistorypost) | **POST** /seo/backlinks/history | Get historical backlink metrics for a target |
| [**SeoBacklinksListPost**](SeoApi.md#seobacklinkslistpost) | **POST** /seo/backlinks/list | List individual backlinks pointing to a target |
| [**SeoBacklinksPageIntersectionPost**](SeoApi.md#seobacklinkspageintersectionpost) | **POST** /seo/backlinks/page-intersection | Find pages linking to multiple targets |
| [**SeoBacklinksReferringDomainsPost**](SeoApi.md#seobacklinksreferringdomainspost) | **POST** /seo/backlinks/referring-domains | List referring domains pointing to a target |
| [**SeoBacklinksReferringNetworksPost**](SeoApi.md#seobacklinksreferringnetworkspost) | **POST** /seo/backlinks/referring-networks | List referring IP networks pointing to a target |
| [**SeoBacklinksSummaryPost**](SeoApi.md#seobacklinkssummarypost) | **POST** /seo/backlinks/summary | Get the backlink profile summary for a target |
| [**SeoBacklinksTimeseriesNewLostPost**](SeoApi.md#seobacklinkstimeseriesnewlostpost) | **POST** /seo/backlinks/timeseries-new-lost | Get new and lost backlinks over time |
| [**SeoBacklinksTimeseriesPost**](SeoApi.md#seobacklinkstimeseriespost) | **POST** /seo/backlinks/timeseries | Get backlink metrics over time |
| [**SeoCompetitorsBulkTrafficPost**](SeoApi.md#seocompetitorsbulktrafficpost) | **POST** /seo/competitors/bulk-traffic | Estimate organic traffic for domains |
| [**SeoCompetitorsDomainIntersectionPost**](SeoApi.md#seocompetitorsdomainintersectionpost) | **POST** /seo/competitors/domain-intersection | Find keywords two domains both rank for |
| [**SeoCompetitorsDomainPost**](SeoApi.md#seocompetitorsdomainpost) | **POST** /seo/competitors/domain | Find a domain&#39;s organic competitors |
| [**SeoCompetitorsDomainRankOverviewPost**](SeoApi.md#seocompetitorsdomainrankoverviewpost) | **POST** /seo/competitors/domain-rank-overview | Get a domain&#39;s ranking and traffic overview |
| [**SeoCompetitorsHistoricalBulkTrafficPost**](SeoApi.md#seocompetitorshistoricalbulktrafficpost) | **POST** /seo/competitors/historical-bulk-traffic | Estimate historical traffic for domains |
| [**SeoCompetitorsHistoricalRankOverviewPost**](SeoApi.md#seocompetitorshistoricalrankoverviewpost) | **POST** /seo/competitors/historical-rank-overview | Get a domain&#39;s historical ranking overview |
| [**SeoCompetitorsHistoricalSerpsPost**](SeoApi.md#seocompetitorshistoricalserpspost) | **POST** /seo/competitors/historical-serps | Get historical SERP snapshots for a keyword |
| [**SeoCompetitorsPageIntersectionPost**](SeoApi.md#seocompetitorspageintersectionpost) | **POST** /seo/competitors/page-intersection | Find keywords specific pages rank for |
| [**SeoCompetitorsRankedKeywordsPost**](SeoApi.md#seocompetitorsrankedkeywordspost) | **POST** /seo/competitors/ranked-keywords | Find the keywords a domain ranks for |
| [**SeoCompetitorsRelevantPagesPost**](SeoApi.md#seocompetitorsrelevantpagespost) | **POST** /seo/competitors/relevant-pages | List a domain&#39;s top ranking pages |
| [**SeoCompetitorsSerpPost**](SeoApi.md#seocompetitorsserppost) | **POST** /seo/competitors/serp | Find domains competing for keywords |
| [**SeoCompetitorsSubdomainsPost**](SeoApi.md#seocompetitorssubdomainspost) | **POST** /seo/competitors/subdomains | List a domain&#39;s subdomains with traffic |
| [**SeoKeywordsAutocompletePost**](SeoApi.md#seokeywordsautocompletepost) | **POST** /seo/keywords/autocomplete | Collect autocomplete keyword suggestions |
| [**SeoKeywordsDifficultyPost**](SeoApi.md#seokeywordsdifficultypost) | **POST** /seo/keywords/difficulty | Score keyword difficulty |
| [**SeoKeywordsForSitePost**](SeoApi.md#seokeywordsforsitepost) | **POST** /seo/keywords/for-site | Find keywords a domain ranks for |
| [**SeoKeywordsHistoryPost**](SeoApi.md#seokeywordshistorypost) | **POST** /seo/keywords/history | Get historical keyword data |
| [**SeoKeywordsIdeasPost**](SeoApi.md#seokeywordsideaspost) | **POST** /seo/keywords/ideas | Discover keyword ideas |
| [**SeoKeywordsIntentPost**](SeoApi.md#seokeywordsintentpost) | **POST** /seo/keywords/intent | Classify keyword search intent |
| [**SeoKeywordsOverviewPost**](SeoApi.md#seokeywordsoverviewpost) | **POST** /seo/keywords/overview | Look up keyword metrics |
| [**SeoKeywordsRelatedPost**](SeoApi.md#seokeywordsrelatedpost) | **POST** /seo/keywords/related | Find related keywords |
| [**SeoKeywordsSuggestionsPost**](SeoApi.md#seokeywordssuggestionspost) | **POST** /seo/keywords/suggestions | Find keyword suggestions |
| [**SeoSerpPost**](SeoApi.md#seoserppost) | **POST** /seo/serp | Collect organic SERP SEO evidence |

<a id="seobacklinksanchorspost"></a>
# **SeoBacklinksAnchorsPost**
> SeoBacklinksAnchorsPost200Response SeoBacklinksAnchorsPost (SeoBacklinksAnchorsRequest? seoBacklinksAnchorsRequest = null)

Get anchor texts used in backlinks to a target

Return the anchor texts used in backlinks pointing to a target, each with backlink, referring-domain, and spam-score counters, to analyze anchor-text distribution.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksAnchorsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksAnchorsRequest = new SeoBacklinksAnchorsRequest?(); // SeoBacklinksAnchorsRequest? |  (optional) 

            try
            {
                // Get anchor texts used in backlinks to a target
                SeoBacklinksAnchorsPost200Response result = apiInstance.SeoBacklinksAnchorsPost(seoBacklinksAnchorsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksAnchorsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksAnchorsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get anchor texts used in backlinks to a target
    ApiResponse<SeoBacklinksAnchorsPost200Response> response = apiInstance.SeoBacklinksAnchorsPostWithHttpInfo(seoBacklinksAnchorsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksAnchorsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksAnchorsRequest** | [**SeoBacklinksAnchorsRequest?**](SeoBacklinksAnchorsRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksAnchorsPost200Response**](SeoBacklinksAnchorsPost200Response.md)

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

<a id="seobacklinksbulkbacklinkspost"></a>
# **SeoBacklinksBulkBacklinksPost**
> SeoBacklinksBulkBacklinksPost200Response SeoBacklinksBulkBacklinksPost (SeoBacklinksBulkBacklinksRequest? seoBacklinksBulkBacklinksRequest = null)

Count backlinks for many targets

Return the total number of backlinks pointing to up to 1000 domains, subdomains, or pages at once, for bulk link-volume comparison.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksBulkBacklinksPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksBulkBacklinksRequest = new SeoBacklinksBulkBacklinksRequest?(); // SeoBacklinksBulkBacklinksRequest? |  (optional) 

            try
            {
                // Count backlinks for many targets
                SeoBacklinksBulkBacklinksPost200Response result = apiInstance.SeoBacklinksBulkBacklinksPost(seoBacklinksBulkBacklinksRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkBacklinksPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksBulkBacklinksPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Count backlinks for many targets
    ApiResponse<SeoBacklinksBulkBacklinksPost200Response> response = apiInstance.SeoBacklinksBulkBacklinksPostWithHttpInfo(seoBacklinksBulkBacklinksRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkBacklinksPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksBulkBacklinksRequest** | [**SeoBacklinksBulkBacklinksRequest?**](SeoBacklinksBulkBacklinksRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksBulkBacklinksPost200Response**](SeoBacklinksBulkBacklinksPost200Response.md)

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

<a id="seobacklinksbulknewlostbacklinkspost"></a>
# **SeoBacklinksBulkNewLostBacklinksPost**
> SeoBacklinksBulkNewLostBacklinksPost200Response SeoBacklinksBulkNewLostBacklinksPost (SeoBacklinksBulkNewLostBacklinksRequest? seoBacklinksBulkNewLostBacklinksRequest = null)

Count new and lost backlinks for many targets

Return the number of new and lost backlinks for up to 1000 domains, subdomains, or pages since a given date, for bulk link-velocity tracking.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksBulkNewLostBacklinksPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksBulkNewLostBacklinksRequest = new SeoBacklinksBulkNewLostBacklinksRequest?(); // SeoBacklinksBulkNewLostBacklinksRequest? |  (optional) 

            try
            {
                // Count new and lost backlinks for many targets
                SeoBacklinksBulkNewLostBacklinksPost200Response result = apiInstance.SeoBacklinksBulkNewLostBacklinksPost(seoBacklinksBulkNewLostBacklinksRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkNewLostBacklinksPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksBulkNewLostBacklinksPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Count new and lost backlinks for many targets
    ApiResponse<SeoBacklinksBulkNewLostBacklinksPost200Response> response = apiInstance.SeoBacklinksBulkNewLostBacklinksPostWithHttpInfo(seoBacklinksBulkNewLostBacklinksRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkNewLostBacklinksPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksBulkNewLostBacklinksRequest** | [**SeoBacklinksBulkNewLostBacklinksRequest?**](SeoBacklinksBulkNewLostBacklinksRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksBulkNewLostBacklinksPost200Response**](SeoBacklinksBulkNewLostBacklinksPost200Response.md)

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

<a id="seobacklinksbulknewlostreferringdomainspost"></a>
# **SeoBacklinksBulkNewLostReferringDomainsPost**
> SeoBacklinksBulkNewLostReferringDomainsPost200Response SeoBacklinksBulkNewLostReferringDomainsPost (SeoBacklinksBulkNewLostReferringDomainsRequest? seoBacklinksBulkNewLostReferringDomainsRequest = null)

Count new and lost referring domains for many targets

Return the number of new and lost referring domains for up to 1000 domains, subdomains, or pages since a given date, for bulk referring-domain velocity tracking.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksBulkNewLostReferringDomainsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksBulkNewLostReferringDomainsRequest = new SeoBacklinksBulkNewLostReferringDomainsRequest?(); // SeoBacklinksBulkNewLostReferringDomainsRequest? |  (optional) 

            try
            {
                // Count new and lost referring domains for many targets
                SeoBacklinksBulkNewLostReferringDomainsPost200Response result = apiInstance.SeoBacklinksBulkNewLostReferringDomainsPost(seoBacklinksBulkNewLostReferringDomainsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkNewLostReferringDomainsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksBulkNewLostReferringDomainsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Count new and lost referring domains for many targets
    ApiResponse<SeoBacklinksBulkNewLostReferringDomainsPost200Response> response = apiInstance.SeoBacklinksBulkNewLostReferringDomainsPostWithHttpInfo(seoBacklinksBulkNewLostReferringDomainsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkNewLostReferringDomainsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksBulkNewLostReferringDomainsRequest** | [**SeoBacklinksBulkNewLostReferringDomainsRequest?**](SeoBacklinksBulkNewLostReferringDomainsRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksBulkNewLostReferringDomainsPost200Response**](SeoBacklinksBulkNewLostReferringDomainsPost200Response.md)

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

<a id="seobacklinksbulkpagessummarypost"></a>
# **SeoBacklinksBulkPagesSummaryPost**
> SeoBacklinksBulkPagesSummaryPost200Response SeoBacklinksBulkPagesSummaryPost (SeoBacklinksBulkPagesSummaryRequest? seoBacklinksBulkPagesSummaryRequest = null)

Summarize backlinks for many pages at once

Return backlink summaries for up to 1000 pages, domains, or subdomains at once, each with backlink, referring-domain, and spam-score counters, for bulk link-profile comparison.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksBulkPagesSummaryPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksBulkPagesSummaryRequest = new SeoBacklinksBulkPagesSummaryRequest?(); // SeoBacklinksBulkPagesSummaryRequest? |  (optional) 

            try
            {
                // Summarize backlinks for many pages at once
                SeoBacklinksBulkPagesSummaryPost200Response result = apiInstance.SeoBacklinksBulkPagesSummaryPost(seoBacklinksBulkPagesSummaryRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkPagesSummaryPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksBulkPagesSummaryPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Summarize backlinks for many pages at once
    ApiResponse<SeoBacklinksBulkPagesSummaryPost200Response> response = apiInstance.SeoBacklinksBulkPagesSummaryPostWithHttpInfo(seoBacklinksBulkPagesSummaryRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkPagesSummaryPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksBulkPagesSummaryRequest** | [**SeoBacklinksBulkPagesSummaryRequest?**](SeoBacklinksBulkPagesSummaryRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksBulkPagesSummaryPost200Response**](SeoBacklinksBulkPagesSummaryPost200Response.md)

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

<a id="seobacklinksbulkrankspost"></a>
# **SeoBacklinksBulkRanksPost**
> SeoBacklinksBulkRanksPost200Response SeoBacklinksBulkRanksPost (SeoBacklinksBulkRanksRequest? seoBacklinksBulkRanksRequest = null)

Get backlink ranks for many targets

Return the backlink rank score (0-1000, similar to PageRank) for up to 1000 domains, subdomains, or pages at once, for quick bulk authority comparison.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksBulkRanksPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksBulkRanksRequest = new SeoBacklinksBulkRanksRequest?(); // SeoBacklinksBulkRanksRequest? |  (optional) 

            try
            {
                // Get backlink ranks for many targets
                SeoBacklinksBulkRanksPost200Response result = apiInstance.SeoBacklinksBulkRanksPost(seoBacklinksBulkRanksRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkRanksPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksBulkRanksPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get backlink ranks for many targets
    ApiResponse<SeoBacklinksBulkRanksPost200Response> response = apiInstance.SeoBacklinksBulkRanksPostWithHttpInfo(seoBacklinksBulkRanksRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkRanksPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksBulkRanksRequest** | [**SeoBacklinksBulkRanksRequest?**](SeoBacklinksBulkRanksRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksBulkRanksPost200Response**](SeoBacklinksBulkRanksPost200Response.md)

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

<a id="seobacklinksbulkreferringdomainspost"></a>
# **SeoBacklinksBulkReferringDomainsPost**
> SeoBacklinksBulkReferringDomainsPost200Response SeoBacklinksBulkReferringDomainsPost (SeoBacklinksBulkReferringDomainsRequest? seoBacklinksBulkReferringDomainsRequest = null)

Count referring domains for many targets

Return the number of referring domains pointing to up to 1000 domains, subdomains, or pages at once, for bulk referring-domain comparison.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksBulkReferringDomainsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksBulkReferringDomainsRequest = new SeoBacklinksBulkReferringDomainsRequest?(); // SeoBacklinksBulkReferringDomainsRequest? |  (optional) 

            try
            {
                // Count referring domains for many targets
                SeoBacklinksBulkReferringDomainsPost200Response result = apiInstance.SeoBacklinksBulkReferringDomainsPost(seoBacklinksBulkReferringDomainsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkReferringDomainsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksBulkReferringDomainsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Count referring domains for many targets
    ApiResponse<SeoBacklinksBulkReferringDomainsPost200Response> response = apiInstance.SeoBacklinksBulkReferringDomainsPostWithHttpInfo(seoBacklinksBulkReferringDomainsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkReferringDomainsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksBulkReferringDomainsRequest** | [**SeoBacklinksBulkReferringDomainsRequest?**](SeoBacklinksBulkReferringDomainsRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksBulkReferringDomainsPost200Response**](SeoBacklinksBulkReferringDomainsPost200Response.md)

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

<a id="seobacklinksbulkspamscorepost"></a>
# **SeoBacklinksBulkSpamScorePost**
> SeoBacklinksBulkSpamScorePost200Response SeoBacklinksBulkSpamScorePost (SeoBacklinksBulkSpamScoreRequest? seoBacklinksBulkSpamScoreRequest = null)

Get spam scores for many targets

Return the DataForSEO spam score (0-100) for up to 1000 domains, subdomains, or pages at once, to flag risky backlink targets in bulk.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksBulkSpamScorePostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksBulkSpamScoreRequest = new SeoBacklinksBulkSpamScoreRequest?(); // SeoBacklinksBulkSpamScoreRequest? |  (optional) 

            try
            {
                // Get spam scores for many targets
                SeoBacklinksBulkSpamScorePost200Response result = apiInstance.SeoBacklinksBulkSpamScorePost(seoBacklinksBulkSpamScoreRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkSpamScorePost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksBulkSpamScorePostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get spam scores for many targets
    ApiResponse<SeoBacklinksBulkSpamScorePost200Response> response = apiInstance.SeoBacklinksBulkSpamScorePostWithHttpInfo(seoBacklinksBulkSpamScoreRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksBulkSpamScorePostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksBulkSpamScoreRequest** | [**SeoBacklinksBulkSpamScoreRequest?**](SeoBacklinksBulkSpamScoreRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksBulkSpamScorePost200Response**](SeoBacklinksBulkSpamScorePost200Response.md)

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

<a id="seobacklinkscompetitorspost"></a>
# **SeoBacklinksCompetitorsPost**
> SeoBacklinksCompetitorsPost200Response SeoBacklinksCompetitorsPost (SeoBacklinksCompetitorsRequest? seoBacklinksCompetitorsRequest = null)

Find competitors by shared referring domains

Return the domains that share referring domains with a target, ranked by the number of shared referring domains, to discover competitors in the same backlink neighborhood.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksCompetitorsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksCompetitorsRequest = new SeoBacklinksCompetitorsRequest?(); // SeoBacklinksCompetitorsRequest? |  (optional) 

            try
            {
                // Find competitors by shared referring domains
                SeoBacklinksCompetitorsPost200Response result = apiInstance.SeoBacklinksCompetitorsPost(seoBacklinksCompetitorsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksCompetitorsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksCompetitorsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find competitors by shared referring domains
    ApiResponse<SeoBacklinksCompetitorsPost200Response> response = apiInstance.SeoBacklinksCompetitorsPostWithHttpInfo(seoBacklinksCompetitorsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksCompetitorsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksCompetitorsRequest** | [**SeoBacklinksCompetitorsRequest?**](SeoBacklinksCompetitorsRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksCompetitorsPost200Response**](SeoBacklinksCompetitorsPost200Response.md)

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

<a id="seobacklinksdomainintersectionpost"></a>
# **SeoBacklinksDomainIntersectionPost**
> SeoBacklinksDomainIntersectionPost200Response SeoBacklinksDomainIntersectionPost (SeoBacklinksDomainIntersectionRequest? seoBacklinksDomainIntersectionRequest = null)

Find domains linking to multiple targets

Return the domains that link to a set of targets, with per-target backlink metrics. Useful for a link-gap analysis: domains linking to competitors but not to your site.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksDomainIntersectionPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksDomainIntersectionRequest = new SeoBacklinksDomainIntersectionRequest?(); // SeoBacklinksDomainIntersectionRequest? |  (optional) 

            try
            {
                // Find domains linking to multiple targets
                SeoBacklinksDomainIntersectionPost200Response result = apiInstance.SeoBacklinksDomainIntersectionPost(seoBacklinksDomainIntersectionRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksDomainIntersectionPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksDomainIntersectionPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find domains linking to multiple targets
    ApiResponse<SeoBacklinksDomainIntersectionPost200Response> response = apiInstance.SeoBacklinksDomainIntersectionPostWithHttpInfo(seoBacklinksDomainIntersectionRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksDomainIntersectionPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksDomainIntersectionRequest** | [**SeoBacklinksDomainIntersectionRequest?**](SeoBacklinksDomainIntersectionRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksDomainIntersectionPost200Response**](SeoBacklinksDomainIntersectionPost200Response.md)

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

<a id="seobacklinksdomainpagespost"></a>
# **SeoBacklinksDomainPagesPost**
> SeoBacklinksDomainPagesPost200Response SeoBacklinksDomainPagesPost (SeoBacklinksDomainPagesRequest? seoBacklinksDomainPagesRequest = null)

List target pages ranked by backlinks

Return the pages of a target domain or subdomain that receive backlinks, each with crawl data and backlink counters, to find the most-linked pages of a site.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksDomainPagesPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksDomainPagesRequest = new SeoBacklinksDomainPagesRequest?(); // SeoBacklinksDomainPagesRequest? |  (optional) 

            try
            {
                // List target pages ranked by backlinks
                SeoBacklinksDomainPagesPost200Response result = apiInstance.SeoBacklinksDomainPagesPost(seoBacklinksDomainPagesRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksDomainPagesPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksDomainPagesPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List target pages ranked by backlinks
    ApiResponse<SeoBacklinksDomainPagesPost200Response> response = apiInstance.SeoBacklinksDomainPagesPostWithHttpInfo(seoBacklinksDomainPagesRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksDomainPagesPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksDomainPagesRequest** | [**SeoBacklinksDomainPagesRequest?**](SeoBacklinksDomainPagesRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksDomainPagesPost200Response**](SeoBacklinksDomainPagesPost200Response.md)

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

<a id="seobacklinksdomainpagessummarypost"></a>
# **SeoBacklinksDomainPagesSummaryPost**
> SeoBacklinksDomainPagesSummaryPost200Response SeoBacklinksDomainPagesSummaryPost (SeoBacklinksDomainPagesSummaryRequest? seoBacklinksDomainPagesSummaryRequest = null)

Summarize backlinks for each page of a target

Return per-page backlink summaries for a target domain or subdomain, each page with backlink, referring-domain, and spam-score counters, to find the most-linked pages.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksDomainPagesSummaryPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksDomainPagesSummaryRequest = new SeoBacklinksDomainPagesSummaryRequest?(); // SeoBacklinksDomainPagesSummaryRequest? |  (optional) 

            try
            {
                // Summarize backlinks for each page of a target
                SeoBacklinksDomainPagesSummaryPost200Response result = apiInstance.SeoBacklinksDomainPagesSummaryPost(seoBacklinksDomainPagesSummaryRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksDomainPagesSummaryPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksDomainPagesSummaryPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Summarize backlinks for each page of a target
    ApiResponse<SeoBacklinksDomainPagesSummaryPost200Response> response = apiInstance.SeoBacklinksDomainPagesSummaryPostWithHttpInfo(seoBacklinksDomainPagesSummaryRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksDomainPagesSummaryPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksDomainPagesSummaryRequest** | [**SeoBacklinksDomainPagesSummaryRequest?**](SeoBacklinksDomainPagesSummaryRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksDomainPagesSummaryPost200Response**](SeoBacklinksDomainPagesSummaryPost200Response.md)

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

<a id="seobacklinkshistorypost"></a>
# **SeoBacklinksHistoryPost**
> SeoBacklinksHistoryPost200Response SeoBacklinksHistoryPost (SeoBacklinksHistoryRequest? seoBacklinksHistoryRequest = null)

Get historical backlink metrics for a target

Return a monthly time series of a target's backlink profile since 2019 — backlinks, referring domains, new/lost counts, and rank — for link-growth trend analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksHistoryPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksHistoryRequest = new SeoBacklinksHistoryRequest?(); // SeoBacklinksHistoryRequest? |  (optional) 

            try
            {
                // Get historical backlink metrics for a target
                SeoBacklinksHistoryPost200Response result = apiInstance.SeoBacklinksHistoryPost(seoBacklinksHistoryRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksHistoryPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksHistoryPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get historical backlink metrics for a target
    ApiResponse<SeoBacklinksHistoryPost200Response> response = apiInstance.SeoBacklinksHistoryPostWithHttpInfo(seoBacklinksHistoryRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksHistoryPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksHistoryRequest** | [**SeoBacklinksHistoryRequest?**](SeoBacklinksHistoryRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksHistoryPost200Response**](SeoBacklinksHistoryPost200Response.md)

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

<a id="seobacklinkslistpost"></a>
# **SeoBacklinksListPost**
> SeoBacklinksListPost200Response SeoBacklinksListPost (SeoBacklinksListRequest? seoBacklinksListRequest = null)

List individual backlinks pointing to a target

Return the individual backlinks pointing to a target domain, subdomain, or page, each with the referring URL, anchor, dofollow flag, rank, and spam score, for detailed link auditing.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksListPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksListRequest = new SeoBacklinksListRequest?(); // SeoBacklinksListRequest? |  (optional) 

            try
            {
                // List individual backlinks pointing to a target
                SeoBacklinksListPost200Response result = apiInstance.SeoBacklinksListPost(seoBacklinksListRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksListPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksListPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List individual backlinks pointing to a target
    ApiResponse<SeoBacklinksListPost200Response> response = apiInstance.SeoBacklinksListPostWithHttpInfo(seoBacklinksListRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksListPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksListRequest** | [**SeoBacklinksListRequest?**](SeoBacklinksListRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksListPost200Response**](SeoBacklinksListPost200Response.md)

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

<a id="seobacklinkspageintersectionpost"></a>
# **SeoBacklinksPageIntersectionPost**
> SeoBacklinksPageIntersectionPost200Response SeoBacklinksPageIntersectionPost (SeoBacklinksPageIntersectionRequest? seoBacklinksPageIntersectionRequest = null)

Find pages linking to multiple targets

Return the referring pages that link to a set of targets, with the backlinks to each target. Useful for finding pages that link to your competitors but not to your site.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksPageIntersectionPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksPageIntersectionRequest = new SeoBacklinksPageIntersectionRequest?(); // SeoBacklinksPageIntersectionRequest? |  (optional) 

            try
            {
                // Find pages linking to multiple targets
                SeoBacklinksPageIntersectionPost200Response result = apiInstance.SeoBacklinksPageIntersectionPost(seoBacklinksPageIntersectionRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksPageIntersectionPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksPageIntersectionPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find pages linking to multiple targets
    ApiResponse<SeoBacklinksPageIntersectionPost200Response> response = apiInstance.SeoBacklinksPageIntersectionPostWithHttpInfo(seoBacklinksPageIntersectionRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksPageIntersectionPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksPageIntersectionRequest** | [**SeoBacklinksPageIntersectionRequest?**](SeoBacklinksPageIntersectionRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksPageIntersectionPost200Response**](SeoBacklinksPageIntersectionPost200Response.md)

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

<a id="seobacklinksreferringdomainspost"></a>
# **SeoBacklinksReferringDomainsPost**
> SeoBacklinksReferringDomainsPost200Response SeoBacklinksReferringDomainsPost (SeoReferringDomainsRequest? seoReferringDomainsRequest = null)

List referring domains pointing to a target

Return the domains that link to a target domain, subdomain, or page, each with backlink, referring-domain, and spam-score counters for referring-domain analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksReferringDomainsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoReferringDomainsRequest = new SeoReferringDomainsRequest?(); // SeoReferringDomainsRequest? |  (optional) 

            try
            {
                // List referring domains pointing to a target
                SeoBacklinksReferringDomainsPost200Response result = apiInstance.SeoBacklinksReferringDomainsPost(seoReferringDomainsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksReferringDomainsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksReferringDomainsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List referring domains pointing to a target
    ApiResponse<SeoBacklinksReferringDomainsPost200Response> response = apiInstance.SeoBacklinksReferringDomainsPostWithHttpInfo(seoReferringDomainsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksReferringDomainsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoReferringDomainsRequest** | [**SeoReferringDomainsRequest?**](SeoReferringDomainsRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksReferringDomainsPost200Response**](SeoBacklinksReferringDomainsPost200Response.md)

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

<a id="seobacklinksreferringnetworkspost"></a>
# **SeoBacklinksReferringNetworksPost**
> SeoBacklinksReferringNetworksPost200Response SeoBacklinksReferringNetworksPost (SeoBacklinksReferringNetworksRequest? seoBacklinksReferringNetworksRequest = null)

List referring IP networks pointing to a target

Return the IP addresses or subnets that host pages linking to a target, each with backlink and referring-domain counters, to assess referring-network diversity.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksReferringNetworksPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksReferringNetworksRequest = new SeoBacklinksReferringNetworksRequest?(); // SeoBacklinksReferringNetworksRequest? |  (optional) 

            try
            {
                // List referring IP networks pointing to a target
                SeoBacklinksReferringNetworksPost200Response result = apiInstance.SeoBacklinksReferringNetworksPost(seoBacklinksReferringNetworksRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksReferringNetworksPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksReferringNetworksPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List referring IP networks pointing to a target
    ApiResponse<SeoBacklinksReferringNetworksPost200Response> response = apiInstance.SeoBacklinksReferringNetworksPostWithHttpInfo(seoBacklinksReferringNetworksRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksReferringNetworksPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksReferringNetworksRequest** | [**SeoBacklinksReferringNetworksRequest?**](SeoBacklinksReferringNetworksRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksReferringNetworksPost200Response**](SeoBacklinksReferringNetworksPost200Response.md)

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

<a id="seobacklinkssummarypost"></a>
# **SeoBacklinksSummaryPost**
> SeoBacklinksSummaryPost200Response SeoBacklinksSummaryPost (SeoBacklinksSummaryRequest? seoBacklinksSummaryRequest = null)

Get the backlink profile summary for a target

Return an overview of a target's backlink profile: total backlinks, referring domains/pages/IPs, rank, spam score, and broken-link counters, for a quick link-profile health check.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksSummaryPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksSummaryRequest = new SeoBacklinksSummaryRequest?(); // SeoBacklinksSummaryRequest? |  (optional) 

            try
            {
                // Get the backlink profile summary for a target
                SeoBacklinksSummaryPost200Response result = apiInstance.SeoBacklinksSummaryPost(seoBacklinksSummaryRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksSummaryPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksSummaryPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get the backlink profile summary for a target
    ApiResponse<SeoBacklinksSummaryPost200Response> response = apiInstance.SeoBacklinksSummaryPostWithHttpInfo(seoBacklinksSummaryRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksSummaryPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksSummaryRequest** | [**SeoBacklinksSummaryRequest?**](SeoBacklinksSummaryRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksSummaryPost200Response**](SeoBacklinksSummaryPost200Response.md)

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

<a id="seobacklinkstimeseriesnewlostpost"></a>
# **SeoBacklinksTimeseriesNewLostPost**
> SeoBacklinksTimeseriesNewLostPost200Response SeoBacklinksTimeseriesNewLostPost (SeoBacklinksTimeseriesNewLostRequest? seoBacklinksTimeseriesNewLostRequest = null)

Get new and lost backlinks over time

Return a time series of new and lost backlinks and referring domains for a target, grouped by day, week, month, or year, for link-velocity analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksTimeseriesNewLostPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksTimeseriesNewLostRequest = new SeoBacklinksTimeseriesNewLostRequest?(); // SeoBacklinksTimeseriesNewLostRequest? |  (optional) 

            try
            {
                // Get new and lost backlinks over time
                SeoBacklinksTimeseriesNewLostPost200Response result = apiInstance.SeoBacklinksTimeseriesNewLostPost(seoBacklinksTimeseriesNewLostRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksTimeseriesNewLostPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksTimeseriesNewLostPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get new and lost backlinks over time
    ApiResponse<SeoBacklinksTimeseriesNewLostPost200Response> response = apiInstance.SeoBacklinksTimeseriesNewLostPostWithHttpInfo(seoBacklinksTimeseriesNewLostRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksTimeseriesNewLostPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksTimeseriesNewLostRequest** | [**SeoBacklinksTimeseriesNewLostRequest?**](SeoBacklinksTimeseriesNewLostRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksTimeseriesNewLostPost200Response**](SeoBacklinksTimeseriesNewLostPost200Response.md)

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

<a id="seobacklinkstimeseriespost"></a>
# **SeoBacklinksTimeseriesPost**
> SeoBacklinksTimeseriesPost200Response SeoBacklinksTimeseriesPost (SeoBacklinksTimeseriesRequest? seoBacklinksTimeseriesRequest = null)

Get backlink metrics over time

Return a time series of a target's backlink metrics grouped by day, week, month, or year between two dates, for tracking backlink and referring-domain trends.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoBacklinksTimeseriesPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBacklinksTimeseriesRequest = new SeoBacklinksTimeseriesRequest?(); // SeoBacklinksTimeseriesRequest? |  (optional) 

            try
            {
                // Get backlink metrics over time
                SeoBacklinksTimeseriesPost200Response result = apiInstance.SeoBacklinksTimeseriesPost(seoBacklinksTimeseriesRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoBacklinksTimeseriesPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoBacklinksTimeseriesPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get backlink metrics over time
    ApiResponse<SeoBacklinksTimeseriesPost200Response> response = apiInstance.SeoBacklinksTimeseriesPostWithHttpInfo(seoBacklinksTimeseriesRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoBacklinksTimeseriesPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBacklinksTimeseriesRequest** | [**SeoBacklinksTimeseriesRequest?**](SeoBacklinksTimeseriesRequest?.md) |  | [optional]  |

### Return type

[**SeoBacklinksTimeseriesPost200Response**](SeoBacklinksTimeseriesPost200Response.md)

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

<a id="seocompetitorsbulktrafficpost"></a>
# **SeoCompetitorsBulkTrafficPost**
> SeoCompetitorsBulkTrafficPost200Response SeoCompetitorsBulkTrafficPost (SeoBulkTrafficRequest? seoBulkTrafficRequest = null)

Estimate organic traffic for domains

Return the estimated monthly organic and paid search traffic for a list of domains, for quick competitor sizing and prospecting across many domains at once.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsBulkTrafficPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoBulkTrafficRequest = new SeoBulkTrafficRequest?(); // SeoBulkTrafficRequest? |  (optional) 

            try
            {
                // Estimate organic traffic for domains
                SeoCompetitorsBulkTrafficPost200Response result = apiInstance.SeoCompetitorsBulkTrafficPost(seoBulkTrafficRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsBulkTrafficPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsBulkTrafficPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Estimate organic traffic for domains
    ApiResponse<SeoCompetitorsBulkTrafficPost200Response> response = apiInstance.SeoCompetitorsBulkTrafficPostWithHttpInfo(seoBulkTrafficRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsBulkTrafficPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoBulkTrafficRequest** | [**SeoBulkTrafficRequest?**](SeoBulkTrafficRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsBulkTrafficPost200Response**](SeoCompetitorsBulkTrafficPost200Response.md)

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

<a id="seocompetitorsdomainintersectionpost"></a>
# **SeoCompetitorsDomainIntersectionPost**
> SeoCompetitorsDomainIntersectionPost200Response SeoCompetitorsDomainIntersectionPost (SeoDomainIntersectionRequest? seoDomainIntersectionRequest = null)

Find keywords two domains both rank for

Return the keywords for which two domains both rank, with each domain's position and URL, to find shared keywords or keyword gaps between competitors.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsDomainIntersectionPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoDomainIntersectionRequest = new SeoDomainIntersectionRequest?(); // SeoDomainIntersectionRequest? |  (optional) 

            try
            {
                // Find keywords two domains both rank for
                SeoCompetitorsDomainIntersectionPost200Response result = apiInstance.SeoCompetitorsDomainIntersectionPost(seoDomainIntersectionRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsDomainIntersectionPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsDomainIntersectionPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find keywords two domains both rank for
    ApiResponse<SeoCompetitorsDomainIntersectionPost200Response> response = apiInstance.SeoCompetitorsDomainIntersectionPostWithHttpInfo(seoDomainIntersectionRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsDomainIntersectionPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoDomainIntersectionRequest** | [**SeoDomainIntersectionRequest?**](SeoDomainIntersectionRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsDomainIntersectionPost200Response**](SeoCompetitorsDomainIntersectionPost200Response.md)

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

<a id="seocompetitorsdomainpost"></a>
# **SeoCompetitorsDomainPost**
> SeoCompetitorsDomainPost200Response SeoCompetitorsDomainPost (SeoCompetitorsDomainRequest? seoCompetitorsDomainRequest = null)

Find a domain's organic competitors

Return the domains that compete with a target domain in organic search, with shared-keyword counts and ranking/traffic metrics, for competitive landscape analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsDomainPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoCompetitorsDomainRequest = new SeoCompetitorsDomainRequest?(); // SeoCompetitorsDomainRequest? |  (optional) 

            try
            {
                // Find a domain's organic competitors
                SeoCompetitorsDomainPost200Response result = apiInstance.SeoCompetitorsDomainPost(seoCompetitorsDomainRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsDomainPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsDomainPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find a domain's organic competitors
    ApiResponse<SeoCompetitorsDomainPost200Response> response = apiInstance.SeoCompetitorsDomainPostWithHttpInfo(seoCompetitorsDomainRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsDomainPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoCompetitorsDomainRequest** | [**SeoCompetitorsDomainRequest?**](SeoCompetitorsDomainRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsDomainPost200Response**](SeoCompetitorsDomainPost200Response.md)

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

<a id="seocompetitorsdomainrankoverviewpost"></a>
# **SeoCompetitorsDomainRankOverviewPost**
> SeoCompetitorsDomainRankOverviewPost200Response SeoCompetitorsDomainRankOverviewPost (SeoDomainRankOverviewRequest? seoDomainRankOverviewRequest = null)

Get a domain's ranking and traffic overview

Return the organic and paid ranking distribution and estimated traffic for a target domain, summarizing how many keywords it ranks for in each position bucket.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsDomainRankOverviewPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoDomainRankOverviewRequest = new SeoDomainRankOverviewRequest?(); // SeoDomainRankOverviewRequest? |  (optional) 

            try
            {
                // Get a domain's ranking and traffic overview
                SeoCompetitorsDomainRankOverviewPost200Response result = apiInstance.SeoCompetitorsDomainRankOverviewPost(seoDomainRankOverviewRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsDomainRankOverviewPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsDomainRankOverviewPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a domain's ranking and traffic overview
    ApiResponse<SeoCompetitorsDomainRankOverviewPost200Response> response = apiInstance.SeoCompetitorsDomainRankOverviewPostWithHttpInfo(seoDomainRankOverviewRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsDomainRankOverviewPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoDomainRankOverviewRequest** | [**SeoDomainRankOverviewRequest?**](SeoDomainRankOverviewRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsDomainRankOverviewPost200Response**](SeoCompetitorsDomainRankOverviewPost200Response.md)

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

<a id="seocompetitorshistoricalbulktrafficpost"></a>
# **SeoCompetitorsHistoricalBulkTrafficPost**
> SeoCompetitorsHistoricalBulkTrafficPost200Response SeoCompetitorsHistoricalBulkTrafficPost (SeoHistoricalBulkTrafficRequest? seoHistoricalBulkTrafficRequest = null)

Estimate historical traffic for domains

Return a monthly estimated organic and paid traffic time series for a list of domains since 2019, for comparing competitor growth trajectories over time.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsHistoricalBulkTrafficPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoHistoricalBulkTrafficRequest = new SeoHistoricalBulkTrafficRequest?(); // SeoHistoricalBulkTrafficRequest? |  (optional) 

            try
            {
                // Estimate historical traffic for domains
                SeoCompetitorsHistoricalBulkTrafficPost200Response result = apiInstance.SeoCompetitorsHistoricalBulkTrafficPost(seoHistoricalBulkTrafficRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsHistoricalBulkTrafficPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsHistoricalBulkTrafficPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Estimate historical traffic for domains
    ApiResponse<SeoCompetitorsHistoricalBulkTrafficPost200Response> response = apiInstance.SeoCompetitorsHistoricalBulkTrafficPostWithHttpInfo(seoHistoricalBulkTrafficRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsHistoricalBulkTrafficPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoHistoricalBulkTrafficRequest** | [**SeoHistoricalBulkTrafficRequest?**](SeoHistoricalBulkTrafficRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsHistoricalBulkTrafficPost200Response**](SeoCompetitorsHistoricalBulkTrafficPost200Response.md)

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

<a id="seocompetitorshistoricalrankoverviewpost"></a>
# **SeoCompetitorsHistoricalRankOverviewPost**
> SeoCompetitorsHistoricalRankOverviewPost200Response SeoCompetitorsHistoricalRankOverviewPost (SeoHistoricalRankOverviewRequest? seoHistoricalRankOverviewRequest = null)

Get a domain's historical ranking overview

Return a monthly time series of a domain's organic and paid ranking distribution and estimated traffic since 2019, for trend and seasonality analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsHistoricalRankOverviewPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoHistoricalRankOverviewRequest = new SeoHistoricalRankOverviewRequest?(); // SeoHistoricalRankOverviewRequest? |  (optional) 

            try
            {
                // Get a domain's historical ranking overview
                SeoCompetitorsHistoricalRankOverviewPost200Response result = apiInstance.SeoCompetitorsHistoricalRankOverviewPost(seoHistoricalRankOverviewRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsHistoricalRankOverviewPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsHistoricalRankOverviewPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get a domain's historical ranking overview
    ApiResponse<SeoCompetitorsHistoricalRankOverviewPost200Response> response = apiInstance.SeoCompetitorsHistoricalRankOverviewPostWithHttpInfo(seoHistoricalRankOverviewRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsHistoricalRankOverviewPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoHistoricalRankOverviewRequest** | [**SeoHistoricalRankOverviewRequest?**](SeoHistoricalRankOverviewRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsHistoricalRankOverviewPost200Response**](SeoCompetitorsHistoricalRankOverviewPost200Response.md)

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

<a id="seocompetitorshistoricalserpspost"></a>
# **SeoCompetitorsHistoricalSerpsPost**
> SeoCompetitorsHistoricalSerpsPost200Response SeoCompetitorsHistoricalSerpsPost (SeoHistoricalSerpsRequest? seoHistoricalSerpsRequest = null)

Get historical SERP snapshots for a keyword

Return historical snapshots of the SERP composition for a keyword since 2019, summarizing how many results and which SERP feature types appeared over time.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsHistoricalSerpsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoHistoricalSerpsRequest = new SeoHistoricalSerpsRequest?(); // SeoHistoricalSerpsRequest? |  (optional) 

            try
            {
                // Get historical SERP snapshots for a keyword
                SeoCompetitorsHistoricalSerpsPost200Response result = apiInstance.SeoCompetitorsHistoricalSerpsPost(seoHistoricalSerpsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsHistoricalSerpsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsHistoricalSerpsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get historical SERP snapshots for a keyword
    ApiResponse<SeoCompetitorsHistoricalSerpsPost200Response> response = apiInstance.SeoCompetitorsHistoricalSerpsPostWithHttpInfo(seoHistoricalSerpsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsHistoricalSerpsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoHistoricalSerpsRequest** | [**SeoHistoricalSerpsRequest?**](SeoHistoricalSerpsRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsHistoricalSerpsPost200Response**](SeoCompetitorsHistoricalSerpsPost200Response.md)

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

<a id="seocompetitorspageintersectionpost"></a>
# **SeoCompetitorsPageIntersectionPost**
> SeoCompetitorsPageIntersectionPost200Response SeoCompetitorsPageIntersectionPost (SeoPageIntersectionRequest? seoPageIntersectionRequest = null)

Find keywords specific pages rank for

Return the keywords that a set of specific page URLs rank for, with each page's position, to analyze keyword overlap across competing pages or your own content.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsPageIntersectionPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoPageIntersectionRequest = new SeoPageIntersectionRequest?(); // SeoPageIntersectionRequest? |  (optional) 

            try
            {
                // Find keywords specific pages rank for
                SeoCompetitorsPageIntersectionPost200Response result = apiInstance.SeoCompetitorsPageIntersectionPost(seoPageIntersectionRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsPageIntersectionPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsPageIntersectionPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find keywords specific pages rank for
    ApiResponse<SeoCompetitorsPageIntersectionPost200Response> response = apiInstance.SeoCompetitorsPageIntersectionPostWithHttpInfo(seoPageIntersectionRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsPageIntersectionPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoPageIntersectionRequest** | [**SeoPageIntersectionRequest?**](SeoPageIntersectionRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsPageIntersectionPost200Response**](SeoCompetitorsPageIntersectionPost200Response.md)

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

<a id="seocompetitorsrankedkeywordspost"></a>
# **SeoCompetitorsRankedKeywordsPost**
> SeoCompetitorsRankedKeywordsPost200Response SeoCompetitorsRankedKeywordsPost (SeoRankedKeywordsRequest? seoRankedKeywordsRequest = null)

Find the keywords a domain ranks for

Return the keywords a target domain or page ranks for in organic search, each with search volume, difficulty, and the exact ranking position and URL, for competitor keyword research.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsRankedKeywordsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoRankedKeywordsRequest = new SeoRankedKeywordsRequest?(); // SeoRankedKeywordsRequest? |  (optional) 

            try
            {
                // Find the keywords a domain ranks for
                SeoCompetitorsRankedKeywordsPost200Response result = apiInstance.SeoCompetitorsRankedKeywordsPost(seoRankedKeywordsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsRankedKeywordsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsRankedKeywordsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find the keywords a domain ranks for
    ApiResponse<SeoCompetitorsRankedKeywordsPost200Response> response = apiInstance.SeoCompetitorsRankedKeywordsPostWithHttpInfo(seoRankedKeywordsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsRankedKeywordsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoRankedKeywordsRequest** | [**SeoRankedKeywordsRequest?**](SeoRankedKeywordsRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsRankedKeywordsPost200Response**](SeoCompetitorsRankedKeywordsPost200Response.md)

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

<a id="seocompetitorsrelevantpagespost"></a>
# **SeoCompetitorsRelevantPagesPost**
> SeoCompetitorsRelevantPagesPost200Response SeoCompetitorsRelevantPagesPost (SeoRelevantPagesRequest? seoRelevantPagesRequest = null)

List a domain's top ranking pages

Return the pages of a target domain that drive the most organic search traffic, each with its ranking distribution and estimated traffic, for content gap and page-level analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsRelevantPagesPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoRelevantPagesRequest = new SeoRelevantPagesRequest?(); // SeoRelevantPagesRequest? |  (optional) 

            try
            {
                // List a domain's top ranking pages
                SeoCompetitorsRelevantPagesPost200Response result = apiInstance.SeoCompetitorsRelevantPagesPost(seoRelevantPagesRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsRelevantPagesPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsRelevantPagesPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a domain's top ranking pages
    ApiResponse<SeoCompetitorsRelevantPagesPost200Response> response = apiInstance.SeoCompetitorsRelevantPagesPostWithHttpInfo(seoRelevantPagesRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsRelevantPagesPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoRelevantPagesRequest** | [**SeoRelevantPagesRequest?**](SeoRelevantPagesRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsRelevantPagesPost200Response**](SeoCompetitorsRelevantPagesPost200Response.md)

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

<a id="seocompetitorsserppost"></a>
# **SeoCompetitorsSerpPost**
> SeoCompetitorsSerpPost200Response SeoCompetitorsSerpPost (SeoSerpCompetitorsRequest? seoSerpCompetitorsRequest = null)

Find domains competing for keywords

Return the domains that rank for a set of seed keywords, ranked by visibility, with average position, estimated traffic, and the number of shared keywords, to discover SERP competitors.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsSerpPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoSerpCompetitorsRequest = new SeoSerpCompetitorsRequest?(); // SeoSerpCompetitorsRequest? |  (optional) 

            try
            {
                // Find domains competing for keywords
                SeoCompetitorsSerpPost200Response result = apiInstance.SeoCompetitorsSerpPost(seoSerpCompetitorsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsSerpPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsSerpPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find domains competing for keywords
    ApiResponse<SeoCompetitorsSerpPost200Response> response = apiInstance.SeoCompetitorsSerpPostWithHttpInfo(seoSerpCompetitorsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsSerpPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoSerpCompetitorsRequest** | [**SeoSerpCompetitorsRequest?**](SeoSerpCompetitorsRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsSerpPost200Response**](SeoCompetitorsSerpPost200Response.md)

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

<a id="seocompetitorssubdomainspost"></a>
# **SeoCompetitorsSubdomainsPost**
> SeoCompetitorsSubdomainsPost200Response SeoCompetitorsSubdomainsPost (SeoSubdomainsRequest? seoSubdomainsRequest = null)

List a domain's subdomains with traffic

Return the subdomains of a target domain, each with its organic ranking distribution and estimated traffic, to see which subdomains drive search visibility.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoCompetitorsSubdomainsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoSubdomainsRequest = new SeoSubdomainsRequest?(); // SeoSubdomainsRequest? |  (optional) 

            try
            {
                // List a domain's subdomains with traffic
                SeoCompetitorsSubdomainsPost200Response result = apiInstance.SeoCompetitorsSubdomainsPost(seoSubdomainsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoCompetitorsSubdomainsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoCompetitorsSubdomainsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // List a domain's subdomains with traffic
    ApiResponse<SeoCompetitorsSubdomainsPost200Response> response = apiInstance.SeoCompetitorsSubdomainsPostWithHttpInfo(seoSubdomainsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoCompetitorsSubdomainsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoSubdomainsRequest** | [**SeoSubdomainsRequest?**](SeoSubdomainsRequest?.md) |  | [optional]  |

### Return type

[**SeoCompetitorsSubdomainsPost200Response**](SeoCompetitorsSubdomainsPost200Response.md)

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

<a id="seokeywordsautocompletepost"></a>
# **SeoKeywordsAutocompletePost**
> SeoKeywordsAutocompletePost200Response SeoKeywordsAutocompletePost (SeoKeywordAutocompleteRequest? seoKeywordAutocompleteRequest = null)

Collect autocomplete keyword suggestions

Run one live autocomplete lookup for a seed query and receive the suggested searches the engine offers, with relevance scores — useful for SEO keyword discovery and content-gap research.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsAutocompletePostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordAutocompleteRequest = new SeoKeywordAutocompleteRequest?(); // SeoKeywordAutocompleteRequest? |  (optional) 

            try
            {
                // Collect autocomplete keyword suggestions
                SeoKeywordsAutocompletePost200Response result = apiInstance.SeoKeywordsAutocompletePost(seoKeywordAutocompleteRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsAutocompletePost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsAutocompletePostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Collect autocomplete keyword suggestions
    ApiResponse<SeoKeywordsAutocompletePost200Response> response = apiInstance.SeoKeywordsAutocompletePostWithHttpInfo(seoKeywordAutocompleteRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsAutocompletePostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordAutocompleteRequest** | [**SeoKeywordAutocompleteRequest?**](SeoKeywordAutocompleteRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsAutocompletePost200Response**](SeoKeywordsAutocompletePost200Response.md)

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

<a id="seokeywordsdifficultypost"></a>
# **SeoKeywordsDifficultyPost**
> SeoKeywordsDifficultyPost200Response SeoKeywordsDifficultyPost (SeoKeywordDifficultyRequest? seoKeywordDifficultyRequest = null)

Score keyword difficulty

Return the keyword difficulty (0-100 chance of ranking in the top-10 organic results) for up to 1,000 keywords in one request, for prioritizing achievable SEO targets.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsDifficultyPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordDifficultyRequest = new SeoKeywordDifficultyRequest?(); // SeoKeywordDifficultyRequest? |  (optional) 

            try
            {
                // Score keyword difficulty
                SeoKeywordsDifficultyPost200Response result = apiInstance.SeoKeywordsDifficultyPost(seoKeywordDifficultyRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsDifficultyPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsDifficultyPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Score keyword difficulty
    ApiResponse<SeoKeywordsDifficultyPost200Response> response = apiInstance.SeoKeywordsDifficultyPostWithHttpInfo(seoKeywordDifficultyRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsDifficultyPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordDifficultyRequest** | [**SeoKeywordDifficultyRequest?**](SeoKeywordDifficultyRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsDifficultyPost200Response**](SeoKeywordsDifficultyPost200Response.md)

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

<a id="seokeywordsforsitepost"></a>
# **SeoKeywordsForSitePost**
> SeoKeywordsForSitePost200Response SeoKeywordsForSitePost (SeoKeywordsForSiteRequest? seoKeywordsForSiteRequest = null)

Find keywords a domain ranks for

Return the keywords a target domain is relevant for, each with search volume, CPC, competition, keyword difficulty, and search intent, for competitor and own-site keyword research.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsForSitePostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordsForSiteRequest = new SeoKeywordsForSiteRequest?(); // SeoKeywordsForSiteRequest? |  (optional) 

            try
            {
                // Find keywords a domain ranks for
                SeoKeywordsForSitePost200Response result = apiInstance.SeoKeywordsForSitePost(seoKeywordsForSiteRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsForSitePost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsForSitePostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find keywords a domain ranks for
    ApiResponse<SeoKeywordsForSitePost200Response> response = apiInstance.SeoKeywordsForSitePostWithHttpInfo(seoKeywordsForSiteRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsForSitePostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordsForSiteRequest** | [**SeoKeywordsForSiteRequest?**](SeoKeywordsForSiteRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsForSitePost200Response**](SeoKeywordsForSitePost200Response.md)

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

<a id="seokeywordshistorypost"></a>
# **SeoKeywordsHistoryPost**
> SeoKeywordsHistoryPost200Response SeoKeywordsHistoryPost (SeoKeywordHistoryRequest? seoKeywordHistoryRequest = null)

Get historical keyword data

Return historical search volume and search ad metrics since 2019 for specified keywords, for trend and seasonality analysis.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsHistoryPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordHistoryRequest = new SeoKeywordHistoryRequest?(); // SeoKeywordHistoryRequest? |  (optional) 

            try
            {
                // Get historical keyword data
                SeoKeywordsHistoryPost200Response result = apiInstance.SeoKeywordsHistoryPost(seoKeywordHistoryRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsHistoryPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsHistoryPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Get historical keyword data
    ApiResponse<SeoKeywordsHistoryPost200Response> response = apiInstance.SeoKeywordsHistoryPostWithHttpInfo(seoKeywordHistoryRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsHistoryPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordHistoryRequest** | [**SeoKeywordHistoryRequest?**](SeoKeywordHistoryRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsHistoryPost200Response**](SeoKeywordsHistoryPost200Response.md)

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

<a id="seokeywordsideaspost"></a>
# **SeoKeywordsIdeasPost**
> SeoKeywordsIdeasPost200Response SeoKeywordsIdeasPost (SeoKeywordIdeasRequest? seoKeywordIdeasRequest = null)

Discover keyword ideas

Expand seed keywords into related search terms that fall into the same product or service categories, each with search volume, CPC, competition, keyword difficulty, and search intent for SEO and content research.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsIdeasPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordIdeasRequest = new SeoKeywordIdeasRequest?(); // SeoKeywordIdeasRequest? |  (optional) 

            try
            {
                // Discover keyword ideas
                SeoKeywordsIdeasPost200Response result = apiInstance.SeoKeywordsIdeasPost(seoKeywordIdeasRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsIdeasPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsIdeasPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Discover keyword ideas
    ApiResponse<SeoKeywordsIdeasPost200Response> response = apiInstance.SeoKeywordsIdeasPostWithHttpInfo(seoKeywordIdeasRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsIdeasPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordIdeasRequest** | [**SeoKeywordIdeasRequest?**](SeoKeywordIdeasRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsIdeasPost200Response**](SeoKeywordsIdeasPost200Response.md)

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

<a id="seokeywordsintentpost"></a>
# **SeoKeywordsIntentPost**
> SeoKeywordsIntentPost200Response SeoKeywordsIntentPost (SeoKeywordIntentRequest? seoKeywordIntentRequest = null)

Classify keyword search intent

Return the search intent (informational, navigational, commercial, or transactional) with probabilities for up to 1,000 keywords, for mapping keywords to the right content type.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsIntentPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordIntentRequest = new SeoKeywordIntentRequest?(); // SeoKeywordIntentRequest? |  (optional) 

            try
            {
                // Classify keyword search intent
                SeoKeywordsIntentPost200Response result = apiInstance.SeoKeywordsIntentPost(seoKeywordIntentRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsIntentPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsIntentPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Classify keyword search intent
    ApiResponse<SeoKeywordsIntentPost200Response> response = apiInstance.SeoKeywordsIntentPostWithHttpInfo(seoKeywordIntentRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsIntentPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordIntentRequest** | [**SeoKeywordIntentRequest?**](SeoKeywordIntentRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsIntentPost200Response**](SeoKeywordsIntentPost200Response.md)

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

<a id="seokeywordsoverviewpost"></a>
# **SeoKeywordsOverviewPost**
> SeoKeywordsOverviewPost200Response SeoKeywordsOverviewPost (SeoKeywordOverviewRequest? seoKeywordOverviewRequest = null)

Look up keyword metrics

Return current SEO metrics for specified keywords, including search volume, CPC, competition, keyword difficulty, and search intent, for prioritizing keyword targets.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsOverviewPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordOverviewRequest = new SeoKeywordOverviewRequest?(); // SeoKeywordOverviewRequest? |  (optional) 

            try
            {
                // Look up keyword metrics
                SeoKeywordsOverviewPost200Response result = apiInstance.SeoKeywordsOverviewPost(seoKeywordOverviewRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsOverviewPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsOverviewPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Look up keyword metrics
    ApiResponse<SeoKeywordsOverviewPost200Response> response = apiInstance.SeoKeywordsOverviewPostWithHttpInfo(seoKeywordOverviewRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsOverviewPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordOverviewRequest** | [**SeoKeywordOverviewRequest?**](SeoKeywordOverviewRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsOverviewPost200Response**](SeoKeywordsOverviewPost200Response.md)

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

<a id="seokeywordsrelatedpost"></a>
# **SeoKeywordsRelatedPost**
> SeoKeywordsRelatedPost200Response SeoKeywordsRelatedPost (SeoRelatedKeywordsRequest? seoRelatedKeywordsRequest = null)

Find related keywords

Expand a seed keyword using the 'searches related to' element, each with search volume, CPC, competition, keyword difficulty, and search intent for SEO and content research.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsRelatedPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoRelatedKeywordsRequest = new SeoRelatedKeywordsRequest?(); // SeoRelatedKeywordsRequest? |  (optional) 

            try
            {
                // Find related keywords
                SeoKeywordsRelatedPost200Response result = apiInstance.SeoKeywordsRelatedPost(seoRelatedKeywordsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsRelatedPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsRelatedPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find related keywords
    ApiResponse<SeoKeywordsRelatedPost200Response> response = apiInstance.SeoKeywordsRelatedPostWithHttpInfo(seoRelatedKeywordsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsRelatedPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoRelatedKeywordsRequest** | [**SeoRelatedKeywordsRequest?**](SeoRelatedKeywordsRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsRelatedPost200Response**](SeoKeywordsRelatedPost200Response.md)

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

<a id="seokeywordssuggestionspost"></a>
# **SeoKeywordsSuggestionsPost**
> SeoKeywordsSuggestionsPost200Response SeoKeywordsSuggestionsPost (SeoKeywordSuggestionsRequest? seoKeywordSuggestionsRequest = null)

Find keyword suggestions

Expand a seed keyword into long-tail search queries that include it, each with search volume, CPC, competition, keyword difficulty, and search intent for SEO and content research.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoKeywordsSuggestionsPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoKeywordSuggestionsRequest = new SeoKeywordSuggestionsRequest?(); // SeoKeywordSuggestionsRequest? |  (optional) 

            try
            {
                // Find keyword suggestions
                SeoKeywordsSuggestionsPost200Response result = apiInstance.SeoKeywordsSuggestionsPost(seoKeywordSuggestionsRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoKeywordsSuggestionsPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoKeywordsSuggestionsPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Find keyword suggestions
    ApiResponse<SeoKeywordsSuggestionsPost200Response> response = apiInstance.SeoKeywordsSuggestionsPostWithHttpInfo(seoKeywordSuggestionsRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoKeywordsSuggestionsPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoKeywordSuggestionsRequest** | [**SeoKeywordSuggestionsRequest?**](SeoKeywordSuggestionsRequest?.md) |  | [optional]  |

### Return type

[**SeoKeywordsSuggestionsPost200Response**](SeoKeywordsSuggestionsPost200Response.md)

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

<a id="seoserppost"></a>
# **SeoSerpPost**
> SeoSerpPost200Response SeoSerpPost (SeoSerpRequest? seoSerpRequest = null)

Collect organic SERP SEO evidence

Run one live organic SERP check for SEO optimization evidence, including target visibility, competitor domains, rich SERP features, People Also Ask context, AI Overview presence, and optional pixel ranking data.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Unifapi.Sdk.Api;
using Unifapi.Sdk.Client;
using Unifapi.Sdk.Model;

namespace Example
{
    public class SeoSerpPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://api.unifapi.com";
            // Configure Bearer token for authorization: bearerAuth
            config.AccessToken = "YOUR_BEARER_TOKEN";

            var apiInstance = new SeoApi(config);
            var seoSerpRequest = new SeoSerpRequest?(); // SeoSerpRequest? |  (optional) 

            try
            {
                // Collect organic SERP SEO evidence
                SeoSerpPost200Response result = apiInstance.SeoSerpPost(seoSerpRequest);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling SeoApi.SeoSerpPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the SeoSerpPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Collect organic SERP SEO evidence
    ApiResponse<SeoSerpPost200Response> response = apiInstance.SeoSerpPostWithHttpInfo(seoSerpRequest);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling SeoApi.SeoSerpPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seoSerpRequest** | [**SeoSerpRequest?**](SeoSerpRequest?.md) |  | [optional]  |

### Return type

[**SeoSerpPost200Response**](SeoSerpPost200Response.md)

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

