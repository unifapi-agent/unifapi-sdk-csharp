# Unifapi.Sdk.Model.SeoBacklinksListResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Target echoed from the request. | 
**View** | **SeoBacklinksView** |  | 
**Mode** | **string** | Result grouping applied to the backlinks. | [optional] 
**TotalCount** | **int** | Total number of backlinks available in DataForSEO&#39;s database. | [optional] 
**SearchAfterToken** | **string** | Token to pass as search_after_token to fetch the next page of backlinks. | [optional] 
**Results** | [**List&lt;SeoBacklinkItem&gt;**](SeoBacklinkItem.md) | Individual backlinks pointing to the target. Each backlink is one billable record. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

