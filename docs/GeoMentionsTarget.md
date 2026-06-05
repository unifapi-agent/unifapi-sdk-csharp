# Unifapi.Sdk.Model.GeoMentionsTarget

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Domain** | **string** | Target domain (no protocol/www). Provide domain or keyword. | [optional] 
**Keyword** | **string** | Target keyword. Provide domain or keyword. | [optional] 
**Filter** | **string** | Whether to include or exclude matches for this entity. Defaults to include. | [optional] 
**Scope** | **List&lt;string&gt;** | Where to look. Domain scopes: any, sources, search_results. Keyword scopes: any, question, answer, brand_entities, fan_out_queries. | [optional] 
**Match** | **string** | Keyword match type. word &#x3D; full-term match; partial &#x3D; substring. Defaults to word. | [optional] 
**IncludeSubdomains** | **bool** | Include subdomains of the target domain. Defaults to false. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

