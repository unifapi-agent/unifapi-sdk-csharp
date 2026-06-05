# Unifapi.Sdk.Model.GeoMentionsAggregatedMetricsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | [**List&lt;GeoMentionsTarget&gt;**](GeoMentionsTarget.md) | Up to 10 target entities, each a domain or a keyword. | 
**Engine** | **GeoEngine** |  | [optional] 
**Location** | [**GeoKeywordSearchVolumeRequestLocation**](GeoKeywordSearchVolumeRequestLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Filters** | [**GeoMentionsAggregatedMetricsRequestFilters**](GeoMentionsAggregatedMetricsRequestFilters.md) |  | [optional] 
**InternalListLimit** | **int** | Max elements per internal grouped array (source/search-result domains). Default 10. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

