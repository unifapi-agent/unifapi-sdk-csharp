# Unifapi.Sdk.Model.SeoBacklinksSummaryRequest

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
**View** | **SeoBacklinksView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

