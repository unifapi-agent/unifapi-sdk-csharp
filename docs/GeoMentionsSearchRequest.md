# Unifapi.Sdk.Model.GeoMentionsSearchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | [**List&lt;GeoMentionsTarget&gt;**](GeoMentionsTarget.md) | Up to 10 target entities, each a domain or a keyword. | 
**Engine** | **GeoEngine** |  | [optional] 
**Location** | [**GeoKeywordSearchVolumeRequestLocation**](GeoKeywordSearchVolumeRequestLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Filters** | [**GeoMentionsSearchRequestFilters**](GeoMentionsSearchRequestFilters.md) |  | [optional] 
**OrderBy** | [**List&lt;DataForSeoOrderByRule&gt;**](DataForSeoOrderByRule.md) | Sort the matched mentions. Each rule is {\&quot;field\&quot;,\&quot;dir\&quot;} with dir asc or desc; up to 3 rules, applied in order. Sortable fields: ai_search_volume, platform, model. | [optional] 
**Limit** | **int** | Max mentions to return. Default 100. | [optional] 
**Offset** | **int** | Mentions to skip. Use cursor beyond 9000. | [optional] 
**Cursor** | **string** | search_after_token from a previous response, for deep pagination. | [optional] 
**View** | **GeoView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

