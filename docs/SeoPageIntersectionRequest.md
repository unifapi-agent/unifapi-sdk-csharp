# Unifapi.Sdk.Model.SeoPageIntersectionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Pages** | **List&lt;string&gt;** | Absolute page URLs to compare (1-20). A trailing /_* wildcard matches a page and its sub-paths. | 
**ExcludePages** | **List&lt;string&gt;** | Page URLs to exclude (up to 10). Keywords where these rank are dropped. | [optional] 
**Location** | [**SeoPageIntersectionLocation**](SeoPageIntersectionLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**IntersectionMode** | **string** | union (default) returns keywords any page ranks for; intersect returns only keywords all pages rank for in the same SERP. | [optional] 
**Limit** | **int** | Maximum number of keywords to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of keywords to skip from the start of the results. | [optional] 
**View** | **SeoKeywordView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

