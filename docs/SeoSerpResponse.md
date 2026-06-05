# Unifapi.Sdk.Model.SeoSerpResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** |  | 
**Location** | **string** |  | 
**Language** | **string** |  | 
**Device** | **string** |  | 
**Os** | **SeoSerpOs** |  | [optional] 
**View** | **SeoSerpView** |  | 
**RankWindow** | [**SeoSerpRankWindow**](SeoSerpRankWindow.md) |  | 
**ObservedAt** | **string** |  | [optional] 
**SearchUrl** | **string** |  | [optional] 
**TotalResults** | **int** |  | [optional] 
**SerpFeatures** | **List&lt;string&gt;** |  | 
**Summary** | [**SeoSerpSummary**](SeoSerpSummary.md) |  | 
**Questions** | [**List&lt;SeoSerpQuestion&gt;**](SeoSerpQuestion.md) | People Also Ask questions useful for SEO content-gap analysis. | 
**Results** | [**List&lt;SeoSerpResult&gt;**](SeoSerpResult.md) | SERP elements returned in source order. Organic results are billable; ads, reviews, people-also-ask, knowledge graph, and other rich elements are returned as free context. | 
**Target** | [**SeoSerpTarget**](SeoSerpTarget.md) |  | [optional] 
**Competitors** | [**List&lt;SeoSerpCompetitor&gt;**](SeoSerpCompetitor.md) | Organic result domains excluding the optional target domain. Omitted when results are truncated by balance. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

