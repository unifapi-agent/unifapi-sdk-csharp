# Unifapi.Sdk.Model.SeoBacklinksListRequestFilters
Filter the returned individual backlinks. Provide a single condition {\"field\",\"op\",\"value\"} or an {\"and\":[…]} / {\"or\":[…]} group of conditions (nest groups for mixed logic), up to 8 conditions. Operators: =, <>, <, <=, >, >=, in, not_in, like, not_like, ilike, not_ilike, match, not_match (use an array value with in / not_in). Filterable fields: domain_from (domain of the referring page); url_from (URL of the referring page); url_to (target URL the backlink points to); domain_to (target domain the backlink points to); dofollow (boolean, link is dofollow); is_new (boolean, appeared since the last check); is_lost (boolean, lost since the last check); is_broken (boolean, points to a broken page); rank (referring page rank, 0-1000); page_from_rank (referring page rank, 0-1000); domain_from_rank (referring domain rank, 0-1000); backlink_spam_score (spam score of the referring page, 0-100); item_type (anchor, image, link, redirect, or canonical); anchor (anchor text); tld_from (top-level domain of the referring page); semantic_location (link location, e.g. article, footer); first_seen (ISO date the backlink was first seen); last_seen (ISO date the backlink was last seen). Example: {\"and\":[{\"field\":\"dofollow\",\"op\":\"=\",\"value\":true},{\"field\":\"is_broken\",\"op\":\"=\",\"value\":false}]}

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Field to filter on. See the endpoint&#39;s list of filterable fields. | 
**Op** | **string** | Comparison operator. | 
**Value** | [**DataForSeoFilterValue**](DataForSeoFilterValue.md) |  | 
**And** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions that must all match. | 
**Or** | [**List&lt;DataForSeoFilter&gt;**](DataForSeoFilter.md) | Sub-expressions where at least one must match. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

