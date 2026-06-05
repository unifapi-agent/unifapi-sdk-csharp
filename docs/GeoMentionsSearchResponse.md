# Unifapi.Sdk.Model.GeoMentionsSearchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Engine** | **GeoEngine** |  | 
**Location** | **string** |  | 
**Language** | **string** |  | 
**TotalCount** | **int** | Total mentions matching the request. | [optional] 
**ReturnedCount** | **int** | Mentions returned in results. | 
**Cursor** | **string** | search_after_token for the next page, when more remain. | [optional] 
**Results** | [**List&lt;GeoMentionRecord&gt;**](GeoMentionRecord.md) | One billable record per matched mention. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

