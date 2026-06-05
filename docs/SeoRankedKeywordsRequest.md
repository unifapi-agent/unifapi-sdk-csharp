# Unifapi.Sdk.Model.SeoRankedKeywordsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Target domain, such as example.com or https://example.com. Specified without www. A page URL can also be passed to get only that page&#39;s rankings. | 
**Location** | [**SeoRankedKeywordsLocation**](SeoRankedKeywordsLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Limit** | **int** | Maximum number of ranked keywords to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of keywords to skip from the start of the results. | [optional] 
**IgnoreSynonyms** | **bool** | When true, exclude highly similar keyword variations from the results. | [optional] 
**View** | **SeoKeywordView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

