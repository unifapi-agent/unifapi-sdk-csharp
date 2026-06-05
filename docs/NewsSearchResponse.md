# Unifapi.Sdk.Model.NewsSearchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** |  | 
**Location** | **string** |  | 
**Language** | **string** |  | 
**View** | **SerpListView** |  | 
**ObservedAt** | **string** |  | [optional] 
**SearchUrl** | **string** |  | [optional] 
**ItemTypes** | **List&lt;string&gt;** | SERP element types present in the result, in source order. | 
**TotalResults** | **int** |  | [optional] 
**ResultCount** | **int** | Number of result elements returned. | 
**Results** | [**List&lt;SerpListElement&gt;**](SerpListElement.md) | News SERP elements in source order. News articles and top-stories blocks are billable; ads are free context. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

