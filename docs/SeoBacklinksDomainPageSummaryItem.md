# Unifapi.Sdk.Model.SeoBacklinksDomainPageSummaryItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | Page URL on the target with its own backlink summary. | 
**Rank** | **int** | Backlink rank of the target, similar to PageRank (0-1000 by default). | [optional] 
**Backlinks** | **int** | Number of backlinks pointing to the target. | [optional] 
**BacklinksSpamScore** | **int** | Average spam score of the referring pages, 0-100. | [optional] 
**FirstSeen** | **string** | Date DataForSEO first found a backlink for the target. | [optional] 
**LostDate** | **string** | Date the last backlink was lost, if the target currently has none. | [optional] 
**BrokenBacklinks** | **int** | Number of backlinks pointing to broken (4xx/5xx) pages of the target. | [optional] 
**BrokenPages** | **int** | Number of broken target pages that still receive backlinks. | [optional] 
**ReferringDomains** | **int** | Number of referring domains pointing to the target. | [optional] 
**ReferringMainDomains** | **int** | Number of referring root domains pointing to the target. | [optional] 
**ReferringPages** | **int** | Number of referring pages pointing to the target. | [optional] 
**ReferringIps** | **int** | Number of referring IP addresses pointing to the target. | [optional] 
**ReferringSubnets** | **int** | Number of referring subnets pointing to the target. | [optional] 
**ReferringDomainsNofollow** | **int** | Referring domains linking only with nofollow backlinks (full view). | [optional] 
**ReferringMainDomainsNofollow** | **int** | Referring root domains linking only with nofollow backlinks (full view). | [optional] 
**ReferringPagesNofollow** | **int** | Referring pages linking only with nofollow backlinks (full view). | [optional] 
**ReferringLinksTld** | **Dictionary&lt;string, int&gt;** | Referring links grouped by top-level domain of the referring page (full view). | [optional] 
**ReferringLinksTypes** | **Dictionary&lt;string, int&gt;** | Referring links grouped by link type, e.g. anchor, image, redirect (full view). | [optional] 
**ReferringLinksAttributes** | **Dictionary&lt;string, int&gt;** | Referring links grouped by link attribute, e.g. nofollow, sponsored, ugc (full view). | [optional] 
**ReferringLinksPlatformTypes** | **Dictionary&lt;string, int&gt;** | Referring links grouped by platform type, e.g. cms, blogs, ecommerce (full view). | [optional] 
**ReferringLinksSemanticLocations** | **Dictionary&lt;string, int&gt;** | Referring links grouped by semantic location on the page, e.g. article, footer (full view). | [optional] 
**ReferringLinksCountries** | **Dictionary&lt;string, int&gt;** | Referring links grouped by country of the referring page (full view). | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

