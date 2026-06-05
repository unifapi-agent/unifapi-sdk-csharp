# Unifapi.Sdk.Model.GeoSerpResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** |  | 
**Location** | **string** |  | 
**Language** | **string** |  | 
**Device** | **string** |  | 
**Surface** | **string** |  | 
**View** | **GeoSerpView** |  | 
**ObservedAt** | **string** |  | [optional] 
**SearchUrl** | **string** |  | [optional] 
**TotalResults** | **int** |  | [optional] 
**SerpFeatures** | **List&lt;string&gt;** |  | 
**Results** | [**List&lt;GeoSerpResult&gt;**](GeoSerpResult.md) | AI SERP elements returned in source order. Top-level AI overview records are billable; cited references, links, images, and answer sections are returned as context inside each result. | 
**Target** | [**GeoSerpTarget**](GeoSerpTarget.md) |  | [optional] 
**Competitors** | [**List&lt;GeoSerpCompetitor&gt;**](GeoSerpCompetitor.md) | Domains cited or linked by AI Mode, excluding the optional target domain. Omitted when results are truncated by balance. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

