# Unifapi.Sdk.Model.SeoBacklinksDomainIntersectionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Targets** | **List&lt;string&gt;** | The requested targets, in request order, echoed back. Each referring_to entry&#39;s target matches one of these. | 
**View** | **SeoBacklinksView** |  | 
**TotalCount** | **int** | Total number of intersecting domains available in DataForSEO&#39;s database. | [optional] 
**Results** | [**List&lt;SeoBacklinksDomainIntersectionItem&gt;**](SeoBacklinksDomainIntersectionItem.md) | Domains that link to the requested targets, with per-target backlink metrics. Each domain is one billable record. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

