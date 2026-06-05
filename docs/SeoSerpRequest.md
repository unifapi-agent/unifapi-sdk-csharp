# Unifapi.Sdk.Model.SeoSerpRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** | Search query to inspect. | 
**Target** | **string** | Optional domain or URL to mark in the results, such as example.com or https://example.com/page. | [optional] 
**Location** | [**SeoSerpLocation**](SeoSerpLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Device** | **string** | SERP device type. Defaults to desktop. | [optional] 
**Os** | **SeoSerpOs** |  | [optional] 
**Page** | **int** | 1-based Google result page to start from. Defaults to 1. Implemented with Google&#39;s start parameter and ranks are adjusted to global SERP positions. | [optional] 
**Depth** | **int** | Organic result depth to crawl from the requested page. Defaults to 10. DataForSEO bills source in 10-result pages; UnifAPI bills returned billable organic records. | [optional] 
**Limit** | **int** | Number of organic results to return, matching the limit parameter used across other UnifAPI endpoints. Maps to DataForSEO depth and is used only when depth is omitted; defaults to 10. | [optional] 
**View** | **SeoSerpView** |  | [optional] 
**IncludeAiOverview** | **bool** | When true, ask DataForSEO to load asynchronous Google AI Overview blocks in the organic SERP when available. This can add source cost. | [optional] 
**PeopleAlsoAskDepth** | **int** | Optional click depth for People Also Ask expansion. Useful for SEO content-gap research and can add source cost. | [optional] 
**IncludePixelRankings** | **bool** | When true, request pixel rectangle data for above-the-fold and visual rank analysis. This can add source cost. | [optional] 
**Viewport** | [**SeoSerpViewport**](SeoSerpViewport.md) |  | [optional] 
**GoogleDomain** | **string** | Optional Google domain override such as google.co.uk or google.de. | [optional] 
**GoogleSearchParams** | **string** | Advanced Google search URL parameters such as nfpr&#x3D;1. Prefer typed fields like page and include_omitted_results when available. | [optional] 
**IncludeOmittedResults** | **bool** | When true, adds filter&#x3D;0 to inspect Google results that may otherwise be omitted. Useful for deep rank checks. | [optional] 
**RemoveUrlParams** | **List&lt;string&gt;** | URL query parameters to remove from result URLs before matching, such as srsltid. | [optional] 
**ExpandRelatedResults** | **bool** | When true, return related/sitelink-style organic results as separate organic elements instead of nesting them. | [optional] 
**StopAtTarget** | **bool** | When true and target is provided, stop crawling once the target is found. Useful for cheaper deep-rank checks, but later competitors may be omitted. | [optional] 
**TargetMatch** | **SeoSerpTargetMatch** |  | [optional] 
**TargetSearchMode** | **SeoSerpTargetSearchMode** |  | [optional] 
**TargetElementTypes** | [**List&lt;SeoSerpTargetElementType&gt;**](SeoSerpTargetElementType.md) | SERP element types to inspect for stop_at_target matches. Defaults to all first-level URL/domain elements. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

