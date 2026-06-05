# Unifapi.Sdk.Model.SeoKeywordIdeasResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SeedKeywords** | **List&lt;string&gt;** | Seed keywords echoed from the request. | 
**Location** | **string** |  | 
**Language** | **string** |  | 
**View** | **SeoKeywordView** |  | 
**TotalCount** | **int** | Total number of keyword ideas available for the request in DataForSEO&#39;s database. | [optional] 
**Offset** | **int** | Offset applied to the results. | [optional] 
**OffsetToken** | **string** | Pass this token as offset_token to fetch the next page of ideas. | [optional] 
**Results** | [**List&lt;SeoKeywordItem&gt;**](SeoKeywordItem.md) | Keyword ideas with search volume, competition, difficulty, and intent. Each keyword is one billable record. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

