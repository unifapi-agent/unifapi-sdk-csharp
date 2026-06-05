# Unifapi.Sdk.Model.LocalFinderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** | Search query to inspect. | 
**Location** | [**SerpListLocation**](SerpListLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Limit** | **int** | Number of results to return, matching the limit parameter used across other UnifAPI endpoints. Maps to result depth. | [optional] 
**View** | **SerpListView** |  | [optional] 
**Device** | **SerpListDevice** |  | [optional] 
**Os** | **SerpListOs** |  | [optional] 
**MinRating** | **decimal** | Filter results to places with at least this average rating. | [optional] 
**TimeFilter** | **string** | Filter results by open hours. open_now keeps only places open at request time. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

