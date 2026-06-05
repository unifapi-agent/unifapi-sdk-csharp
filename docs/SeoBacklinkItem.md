# Unifapi.Sdk.Model.SeoBacklinkItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DomainFrom** | **string** | Domain of the page that links to the target. | [optional] 
**UrlFrom** | **string** | URL of the page that links to the target. | [optional] 
**UrlTo** | **string** | Target URL the backlink points to. | [optional] 
**DomainTo** | **string** | Target domain the backlink points to. | [optional] 
**Anchor** | **string** | Anchor text of the backlink. | [optional] 
**Dofollow** | **bool** | Whether the backlink is dofollow. | [optional] 
**ItemType** | **string** | Type of backlink: anchor, image, link, redirect, or canonical. | [optional] 
**Rank** | **int** | Backlink rank of the referring page (0-1000). | [optional] 
**PageFromRank** | **int** | Rank of the referring page itself (0-1000). | [optional] 
**DomainFromRank** | **int** | Rank of the referring domain (0-1000). | [optional] 
**BacklinkSpamScore** | **int** | Spam score of the referring page, 0-100. | [optional] 
**IsNew** | **bool** | Whether the backlink appeared since the last check. | [optional] 
**IsLost** | **bool** | Whether the backlink was lost since the last check. | [optional] 
**IsBroken** | **bool** | Whether the backlink points to a broken page. | [optional] 
**FirstSeen** | **string** | Date the backlink was first found. | [optional] 
**LastSeen** | **string** | Date the backlink was last seen. | [optional] 
**PrevSeen** | **string** | Previous date the backlink was seen before the last check (full view). | [optional] 
**TldFrom** | **string** | Top-level domain of the referring page (full view). | [optional] 
**UrlFromHttps** | **bool** | Whether the referring page uses HTTPS (full view). | [optional] 
**UrlToHttps** | **bool** | Whether the target URL uses HTTPS (full view). | [optional] 
**Alt** | **string** | Alt text, if the backlink is an image link (full view). | [optional] 
**ImageUrl** | **string** | Image URL, if the backlink is an image link (full view). | [optional] 
**TextPre** | **string** | Text immediately before the anchor (full view). | [optional] 
**TextPost** | **string** | Text immediately after the anchor (full view). | [optional] 
**SemanticLocation** | **string** | Semantic location of the link on the page, e.g. article, footer (full view). | [optional] 
**Attributes** | **List&lt;string&gt;** | Link rel attributes, e.g. nofollow, sponsored, ugc (full view). | [optional] 
**LinksCount** | **int** | Number of identical links from the referring page (full view). | [optional] 
**GroupCount** | **int** | Number of similar grouped links from the referring domain (full view). | [optional] 
**PageFromTitle** | **string** | Title of the referring page (full view). | [optional] 
**PageFromLanguage** | **string** | Language of the referring page (full view). | [optional] 
**PageFromStatusCode** | **int** | HTTP status code of the referring page (full view). | [optional] 
**PageFromExternalLinks** | **int** | Number of external links on the referring page (full view). | [optional] 
**PageFromInternalLinks** | **int** | Number of internal links on the referring page (full view). | [optional] 
**DomainFromCountry** | **string** | Country of the referring domain (full view). | [optional] 
**DomainFromPlatformType** | **List&lt;string&gt;** | Platform types of the referring domain, e.g. cms, blogs (full view). | [optional] 
**UrlToStatusCode** | **int** | HTTP status code of the target URL (full view). | [optional] 
**UrlToRedirectTarget** | **string** | Redirect target of the backlink URL, if any (full view). | [optional] 
**IsIndirectLink** | **bool** | Whether the link reaches the target via a redirect or canonical (full view). | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

