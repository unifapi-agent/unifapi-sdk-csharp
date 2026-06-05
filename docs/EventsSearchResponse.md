# Unifapi.Sdk.Model.EventsSearchResponse

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
**Results** | [**List&lt;SerpListElement&gt;**](SerpListElement.md) | Individual events results flattened from the events block. Each event is one billable record; date, venue, and ticket details are carried in extras. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

