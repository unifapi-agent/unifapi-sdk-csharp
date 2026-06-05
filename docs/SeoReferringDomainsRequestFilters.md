# Unifapi.Sdk.Model.SeoReferringDomainsRequestFilters
Filter the returned referring domains. Provide a single condition {\"field\",\"op\",\"value\"} or an {\"and\":[…]} / {\"or\":[…]} group of conditions (nest groups for mixed logic), up to 8 conditions. Operators: =, <>, <, <=, >, >=, in, not_in, like, not_like, ilike, not_ilike, match, not_match (use an array value with in / not_in). Filterable fields: domain (referring domain); rank (backlink rank, 0-1000); backlinks (number of backlinks); backlinks_spam_score (average spam score, 0-100); referring_domains (referring domains count); referring_main_domains (referring root domains count); referring_pages (referring pages count); referring_ips (referring IPs count); referring_subnets (referring subnets count); broken_backlinks (backlinks to broken pages); broken_pages (broken pages still receiving backlinks); first_seen (ISO date the first backlink was found); lost_date (ISO date the last backlink was lost). Example: {\"and\":[{\"field\":\"rank\",\"op\":\">\",\"value\":200},{\"field\":\"backlinks\",\"op\":\">\",\"value\":10}]}

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Field to filter on. See the endpoint&#39;s list of filterable fields. | 
**Op** | **string** | Comparison operator. | 
**Value** | [**DataForSeoFilterValue**](DataForSeoFilterValue.md) |  | 
**And** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions that must all match. | 
**Or** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions where at least one must match. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

