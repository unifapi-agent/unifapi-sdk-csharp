# Unifapi.Sdk.Model.SeoDomainIntersectionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target1** | **string** | First domain, such as example.com. | 
**Target2** | **string** | Second domain to compare against. | 
**Location** | [**SeoDomainIntersectionLocation**](SeoDomainIntersectionLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Intersections** | **bool** | When true (default), return keywords both domains rank for. When false, return keywords the first domain ranks for but the second does not. | [optional] 
**Limit** | **int** | Maximum number of keywords to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of keywords to skip from the start of the results. | [optional] 
**View** | **SeoKeywordView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

