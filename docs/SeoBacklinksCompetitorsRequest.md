# Unifapi.Sdk.Model.SeoBacklinksCompetitorsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Domain, subdomain, or page to analyze. A domain or subdomain is specified without https:// and www. (example.com); a page is specified as an absolute URL (https://example.com/blog/). | 
**MainDomain** | **bool** | Treat the target and competitors as root domains rather than exact subdomains. | [optional] 
**ExcludeLargeDomains** | **bool** | Exclude very large generic domains (e.g. youtube.com, facebook.com) from results. | [optional] 
**ExcludeInternalBacklinks** | **bool** | Exclude internal backlinks from the target&#39;s own subdomains. Defaults to true. | [optional] 
**RankScale** | **SeoBacklinksRankScale** |  | [optional] 
**Filters** | [**SeoBacklinksCompetitorsRequestFilters**](SeoBacklinksCompetitorsRequestFilters.md) |  | [optional] 
**OrderBy** | [**List&lt;DataForSeoOrderByRule&gt;**](DataForSeoOrderByRule.md) | Sort the returned competitors. Each rule is {\&quot;field\&quot;,\&quot;dir\&quot;} with dir asc or desc; up to 3 rules, applied in order. Sortable fields: rank, intersections. | [optional] 
**Limit** | **int** | Maximum number of records to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of records to skip from the start of the results. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

