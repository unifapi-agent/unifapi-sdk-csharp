# Unifapi.Sdk.Model.SeoBacklinksAnchorsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Domain, subdomain, or page to analyze. A domain or subdomain is specified without https:// and www. (example.com); a page is specified as an absolute URL (https://example.com/blog/). | 
**BacklinksStatusType** | **SeoBacklinksStatusType** |  | [optional] 
**IncludeSubdomains** | **bool** | Include backlinks pointing to the target&#39;s subdomains. Defaults to true. | [optional] 
**IncludeIndirectLinks** | **bool** | Include indirect links (via redirects or canonicals) to the target. Defaults to true. | [optional] 
**ExcludeInternalBacklinks** | **bool** | Exclude internal backlinks from the target&#39;s own subdomains. Defaults to true. | [optional] 
**InternalListLimit** | **int** | Maximum number of entries kept in each referring_links_* breakdown map. Defaults to 10. | [optional] 
**RankScale** | **SeoBacklinksRankScale** |  | [optional] 
**Filters** | [**SeoBacklinksAnchorsRequestFilters**](SeoBacklinksAnchorsRequestFilters.md) |  | [optional] 
**BacklinksFilters** | [**SeoBacklinksAnchorsRequestBacklinksFilters**](SeoBacklinksAnchorsRequestBacklinksFilters.md) |  | [optional] 
**OrderBy** | [**List&lt;DataForSeoOrderByRule&gt;**](DataForSeoOrderByRule.md) | Sort the returned anchors. Each rule is {\&quot;field\&quot;,\&quot;dir\&quot;} with dir asc or desc; up to 3 rules, applied in order. Sortable fields: anchor, rank, backlinks, backlinks_spam_score, referring_domains, referring_main_domains, referring_pages, referring_ips, referring_subnets, broken_backlinks, broken_pages, first_seen, lost_date. | [optional] 
**Limit** | **int** | Maximum number of records to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of records to skip from the start of the results. | [optional] 
**View** | **SeoBacklinksView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

