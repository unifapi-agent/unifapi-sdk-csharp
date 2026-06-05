# Unifapi.Sdk.Model.SeoBacklinksPageIntersectionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Targets** | **List&lt;string&gt;** | The requested targets, in request order, echoed back. Each links_to entry&#39;s target matches one of these. | 
**View** | **SeoBacklinksView** |  | 
**TotalCount** | **int** | Total number of intersecting pages available in DataForSEO&#39;s database. | [optional] 
**Results** | [**List&lt;SeoBacklinksPageIntersectionItem&gt;**](SeoBacklinksPageIntersectionItem.md) | Referring pages that link to the requested targets, with the backlinks to each target. Each page is one billable record. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

