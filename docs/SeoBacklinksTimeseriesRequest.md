# Unifapi.Sdk.Model.SeoBacklinksTimeseriesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Domain, subdomain, or page to analyze. A domain or subdomain is specified without https:// and www. (example.com); a page is specified as an absolute URL (https://example.com/blog/). | 
**DateFrom** | **string** | Start date (yyyy-mm-dd) for the series. Minimum 2019-01-30; defaults to one month ago. | [optional] 
**DateTo** | **string** | End date (yyyy-mm-dd). Defaults to today. | [optional] 
**GroupRange** | **string** | Granularity used to group the series. Defaults to month. | [optional] 
**IncludeSubdomains** | **bool** | Include backlinks pointing to the target&#39;s subdomains. Defaults to true. | [optional] 
**RankScale** | **SeoBacklinksRankScale** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

