# Unifapi.Sdk.Model.SeoKeywordsForSiteResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Target domain echoed from the request. | 
**Location** | **string** |  | 
**Language** | **string** |  | 
**View** | **SeoKeywordView** |  | 
**TotalCount** | **int** | Total number of keywords available for the target in DataForSEO&#39;s database. | [optional] 
**Offset** | **int** | Offset applied to the results. | [optional] 
**OffsetToken** | **string** | Pass this token as offset_token to fetch the next page of keywords. | [optional] 
**Results** | [**List&lt;SeoKeywordItem&gt;**](SeoKeywordItem.md) | Keywords the domain is relevant for, with search volume, competition, difficulty, and intent. Each keyword is one billable record. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

