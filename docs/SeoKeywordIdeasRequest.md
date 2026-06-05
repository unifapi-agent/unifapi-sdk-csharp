# Unifapi.Sdk.Model.SeoKeywordIdeasRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Keywords** | **List&lt;string&gt;** | Seed keywords (1-200). Returns search terms relevant to the product or service categories of these keywords. | 
**Location** | [**SeoKeywordIdeasLocation**](SeoKeywordIdeasLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Limit** | **int** | Maximum number of keyword ideas to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of keyword ideas to skip from the start of the results. | [optional] 
**OffsetToken** | **string** | Pagination token from a previous response. When set, all other params except limit are ignored. | [optional] 
**CloselyVariants** | **bool** | When true, use phrase-match search; when false (default), use broad-match search for wider ideas. | [optional] 
**IgnoreSynonyms** | **bool** | When true, exclude highly similar keywords and return only core keywords. | [optional] 
**IncludeSerpInfo** | **bool** | When true, include SERP data (result count and SERP feature types) for each keyword. Can add source cost. | [optional] 
**View** | **SeoKeywordView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

