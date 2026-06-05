# Unifapi.Sdk.Model.SeoRelatedKeywordsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Keyword** | **string** | Seed keyword. Returns keywords from Google&#39;s &#39;searches related to&#39; element. | 
**Location** | [**SeoRelatedKeywordsLocation**](SeoRelatedKeywordsLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Depth** | **int** | Keyword search depth, 0-4. Higher depth returns more keywords (1≈8, 2≈72, 3≈584, 4≈4680). Defaults to 1. | [optional] 
**Limit** | **int** | Maximum number of related keywords to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of related keywords to skip from the start of the results. | [optional] 
**IgnoreSynonyms** | **bool** | When true, exclude highly similar keywords and return only core keywords. | [optional] 
**IncludeSerpInfo** | **bool** | When true, include SERP data (result count and SERP feature types) for each keyword. Can add source cost. | [optional] 
**IncludeSeedKeyword** | **bool** | When true, include metrics for the seed keyword in the response. | [optional] 
**View** | **SeoKeywordView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

