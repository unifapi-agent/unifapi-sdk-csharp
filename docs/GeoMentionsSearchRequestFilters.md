# Unifapi.Sdk.Model.GeoMentionsSearchRequestFilters
Filter the matched mentions. Provide a single condition {\"field\",\"op\",\"value\"} or an {\"and\":[…]} / {\"or\":[…]} group of conditions (nest groups for mixed logic), up to 8 conditions. Operators: =, <>, <, <=, >, >=, in, not_in, like, not_like, ilike, not_ilike, match, not_match (use an array value with in / not_in). Filterable fields: ai_search_volume (monthly AI search volume); platform (LLM engine, e.g. chat_gpt, google, perplexity); model (model name that produced the answer). Example: {\"and\":[{\"field\":\"ai_search_volume\",\"op\":\">\",\"value\":1000},{\"field\":\"platform\",\"op\":\"=\",\"value\":\"chat_gpt\"}]}

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Field to filter on. See the endpoint&#39;s list of filterable fields. | 
**Op** | **string** | Comparison operator. | 
**Value** | [**DataForSeoFilterValue**](DataForSeoFilterValue.md) |  | 
**And** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions that must all match. | 
**Or** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions where at least one must match. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

