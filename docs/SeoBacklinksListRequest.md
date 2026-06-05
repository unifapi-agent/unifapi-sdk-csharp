# Unifapi.Sdk.Model.SeoBacklinksListRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Domain, subdomain, or page to analyze. A domain or subdomain is specified without https:// and www. (example.com); a page is specified as an absolute URL (https://example.com/blog/). | 
**Mode** | **string** | Result grouping: as_is returns every backlink (default), one_per_domain returns one per referring domain, one_per_anchor returns one per anchor. | [optional] 
**BacklinksStatusType** | **SeoBacklinksStatusType** |  | [optional] 
**IncludeSubdomains** | **bool** | Include backlinks pointing to the target&#39;s subdomains. Defaults to true. | [optional] 
**IncludeIndirectLinks** | **bool** | Include indirect links (via redirects or canonicals) to the target. Defaults to true. | [optional] 
**ExcludeInternalBacklinks** | **bool** | Exclude internal backlinks from the target&#39;s own subdomains. Defaults to true. | [optional] 
**RankScale** | **SeoBacklinksRankScale** |  | [optional] 
**Filters** | [**SeoBacklinksListRequestFilters**](SeoBacklinksListRequestFilters.md) |  | [optional] 
**OrderBy** | [**List&lt;DataForSeoOrderByRule&gt;**](DataForSeoOrderByRule.md) | Sort the returned backlinks. Each rule is {\&quot;field\&quot;,\&quot;dir\&quot;} with dir asc or desc; up to 3 rules, applied in order. Sortable fields: domain_from, url_from, url_to, domain_to, dofollow, is_new, is_lost, is_broken, rank, page_from_rank, domain_from_rank, backlink_spam_score, item_type, anchor, tld_from, semantic_location, first_seen, last_seen. | [optional] 
**Limit** | **int** | Maximum number of records to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of records to skip from the start of the results. | [optional] 
**SearchAfterToken** | **string** | Continuation token from a previous response, used to page past the 20,000-result offset limit. Keep all other parameters identical when paging. | [optional] 
**View** | **SeoBacklinksView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

