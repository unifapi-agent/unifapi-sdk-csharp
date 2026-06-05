# Unifapi.Sdk.Model.SeoKeywordSuggestionsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Keyword** | **string** | Seed keyword. Returns long-tail search queries that include this keyword. | 
**Location** | [**SeoKeywordSuggestionsLocation**](SeoKeywordSuggestionsLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Limit** | **int** | Maximum number of keyword suggestions to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of keyword suggestions to skip from the start of the results. | [optional] 
**OffsetToken** | **string** | Pagination token from a previous response. When set, all other params except limit are ignored. | [optional] 
**ExactMatch** | **bool** | When true, return only suggestions that contain the exact seed keyword in the same word order. | [optional] 
**IgnoreSynonyms** | **bool** | When true, exclude highly similar keywords and return only core keywords. | [optional] 
**IncludeSerpInfo** | **bool** | When true, include SERP data (result count and SERP feature types) for each keyword. Can add source cost. | [optional] 
**IncludeSeedKeyword** | **bool** | When true, include metrics for the seed keyword in the response. | [optional] 
**View** | **SeoKeywordView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

