# Unifapi.Sdk.Model.SeoBacklinksCompetitorsRequestFilters
Filter the returned competitors. Provide a single condition {\"field\",\"op\",\"value\"} or an {\"and\":[…]} / {\"or\":[…]} group of conditions (nest groups for mixed logic), up to 8 conditions. Operators: =, <>, <, <=, >, >=, in, not_in, like, not_like, ilike, not_ilike, match, not_match (use an array value with in / not_in). Filterable fields: rank (backlink rank of the competing domain, 0-1000); intersections (referring domains shared with the target). Example: {\"field\":\"intersections\",\"op\":\">\",\"value\":20}

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Field to filter on. See the endpoint&#39;s list of filterable fields. | 
**Op** | **string** | Comparison operator. | 
**Value** | [**DataForSeoFilterValue**](DataForSeoFilterValue.md) |  | 
**And** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions that must all match. | 
**Or** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions where at least one must match. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

