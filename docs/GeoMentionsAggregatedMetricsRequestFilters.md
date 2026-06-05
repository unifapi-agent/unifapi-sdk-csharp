# Unifapi.Sdk.Model.GeoMentionsAggregatedMetricsRequestFilters
Filter the raw mentions dataset before it is aggregated. Provide a single condition {\"field\",\"op\",\"value\"} or an {\"and\":[…]} / {\"or\":[…]} group of conditions (nest groups for mixed logic), up to 8 conditions. Operators: =, <>, <, <=, >, >=, in, not_in, like, not_like, ilike, not_ilike, match, not_match (use an array value with in / not_in). Filterable fields: ai_search_volume (monthly AI search volume); mentions (number of mentions); platform (LLM engine, e.g. chat_gpt, google); location (location name); language (language name); sources_domain (cited source domain); search_results_domain (domain in the engine's search results); brand_entities_title (brand entity title); brand_entities_category (brand entity category). Example: {\"field\":\"ai_search_volume\",\"op\":\">\",\"value\":1000}

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Field to filter on. See the endpoint&#39;s list of filterable fields. | 
**Op** | **string** | Comparison operator. | 
**Value** | [**DataForSeoFilterValue**](DataForSeoFilterValue.md) |  | 
**And** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions that must all match. | 
**Or** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions where at least one must match. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

