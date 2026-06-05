# Unifapi.Sdk.Model.GeoMentionsTopPagesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | [**List&lt;GeoMentionsTarget&gt;**](GeoMentionsTarget.md) | Up to 10 target entities, each a domain or a keyword. | 
**Engine** | **GeoEngine** |  | [optional] 
**Location** | [**GeoKeywordSearchVolumeRequestLocation**](GeoKeywordSearchVolumeRequestLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**LinksScope** | **string** | Which links to extract pages from. Defaults to sources. | [optional] 
**Filters** | [**GeoMentionsAggregatedMetricsRequestFilters**](GeoMentionsAggregatedMetricsRequestFilters.md) |  | [optional] 
**ItemsListLimit** | **int** | Max number of top pages to return. Default 5. | [optional] 
**InternalListLimit** | **int** | Max elements per internal grouped array. Default 5. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

