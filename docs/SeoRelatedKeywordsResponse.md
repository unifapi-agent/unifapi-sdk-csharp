# Unifapi.Sdk.Model.SeoRelatedKeywordsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SeedKeyword** | **string** | Seed keyword echoed from the request. | 
**Location** | **string** |  | 
**Language** | **string** |  | 
**View** | **SeoKeywordView** |  | 
**TotalCount** | **int** | Total number of related keywords available for the request in DataForSEO&#39;s database. | [optional] 
**Offset** | **int** | Offset applied to the results. | [optional] 
**Results** | [**List&lt;SeoRelatedKeywordItem&gt;**](SeoRelatedKeywordItem.md) | Related keywords with search volume, competition, difficulty, intent, and their own related searches. Each keyword is one billable record. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

