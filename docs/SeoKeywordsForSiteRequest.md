# Unifapi.Sdk.Model.SeoKeywordsForSiteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Target domain, such as example.com or https://example.com. Returns keywords the domain is relevant for. | 
**Location** | [**SeoKeywordsForSiteLocation**](SeoKeywordsForSiteLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Limit** | **int** | Maximum number of keywords to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of keywords to skip from the start of the results. | [optional] 
**OffsetToken** | **string** | Pagination token from a previous response. When set, all other params except limit are ignored. | [optional] 
**IncludeSubdomains** | **bool** | When true (default), include keywords from subdomains of the target. | [optional] 
**IncludeSerpInfo** | **bool** | When true, include SERP data (result count and SERP feature types) for each keyword. Can add source cost. | [optional] 
**View** | **SeoKeywordView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

