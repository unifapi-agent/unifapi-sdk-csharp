# Unifapi.Sdk.Model.SeoBacklinksPageIntersectionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Targets** | **List&lt;string&gt;** | Domains, subdomains, or pages to find common referring pages for (1-20). Order is preserved as the 1-based index in the response. | 
**ExcludeTargets** | **List&lt;string&gt;** | Domains, subdomains, or pages to exclude (up to 10). Pages linking to these are dropped. | [optional] 
**IntersectionMode** | **string** | all (default) returns pages linking to any target; partial returns only pages linking to every target. | [optional] 
**BacklinksStatusType** | **SeoBacklinksStatusType** |  | [optional] 
**IncludeSubdomains** | **bool** | Include backlinks pointing to the target&#39;s subdomains. Defaults to true. | [optional] 
**IncludeIndirectLinks** | **bool** | Include indirect links (via redirects or canonicals) to the target. Defaults to true. | [optional] 
**ExcludeInternalBacklinks** | **bool** | Exclude internal backlinks from the target&#39;s own subdomains. Defaults to true. | [optional] 
**InternalListLimit** | **int** | Maximum number of entries kept in each referring_links_* breakdown map. Defaults to 10. | [optional] 
**RankScale** | **SeoBacklinksRankScale** |  | [optional] 
**Filters** | [**SeoBacklinksPageIntersectionRequestFilters**](SeoBacklinksPageIntersectionRequestFilters.md) |  | [optional] 
**OrderBy** | [**List&lt;DataForSeoOrderByRule&gt;**](DataForSeoOrderByRule.md) | Sort the intersecting referring pages. Prefix each field with the 1-based target index, e.g. 1.rank. Each rule is {\&quot;field\&quot;,\&quot;dir\&quot;} with dir asc or desc; up to 3 rules, applied in order. Sortable fields: dofollow, is_new, is_lost, is_broken, rank, page_from_rank, domain_from_rank, backlink_spam_score, item_type, anchor, tld_from, semantic_location, first_seen, last_seen. | [optional] 
**Limit** | **int** | Maximum number of records to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of records to skip from the start of the results. | [optional] 
**View** | **SeoBacklinksView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

