# Unifapi.Sdk.Model.EventsSearchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** | Search query to inspect. | 
**Location** | [**SerpListLocation**](SerpListLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Limit** | **int** | Number of results to return, matching the limit parameter used across other UnifAPI endpoints. Maps to result depth. | [optional] 
**View** | **SerpListView** |  | [optional] 
**Os** | **SerpListOs** |  | [optional] 
**DateRange** | **string** | Restrict events to a relative date range. Defaults to all upcoming events. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

