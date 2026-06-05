# Unifapi.Sdk.Model.SeoRelatedKeywordItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Keyword** | **string** | Keyword phrase. | 
**SearchVolume** | **int** | Average monthly Google search volume. | [optional] 
**Cpc** | **decimal** | Average cost-per-click in USD. | [optional] 
**Competition** | **decimal** | Google Ads competition index between 0 and 1. | [optional] 
**CompetitionLevel** | **string** | Google Ads competition level: LOW, MEDIUM, or HIGH. | [optional] 
**KeywordDifficulty** | **int** | Relative difficulty of ranking in the top-10 organic results, 0-100. | [optional] 
**SearchIntent** | **string** | Main search intent: informational, navigational, commercial, or transactional. | [optional] 
**SearchIntentAlternatives** | **List&lt;string&gt;** | Supplementary search intents detected for the keyword. | [optional] 
**LowTopOfPageBid** | **decimal** | Lower-range top-of-page bid in USD from Google Ads. | [optional] 
**HighTopOfPageBid** | **decimal** | Upper-range top-of-page bid in USD from Google Ads. | [optional] 
**WordsCount** | **int** | Number of words in the keyword. | [optional] 
**DetectedLanguage** | **string** | Language detected for the keyword. | [optional] 
**SearchVolumeTrend** | [**SeoKeywordSearchVolumeTrend**](SeoKeywordSearchVolumeTrend.md) |  | [optional] 
**SerpItemTypes** | **List&lt;string&gt;** | SERP feature types present for the keyword (only with include_serp_info). | [optional] 
**SerpResultsCount** | **int** | Number of organic results Google reports for the keyword. | [optional] 
**MonthlySearches** | [**List&lt;SeoKeywordMonthlySearch&gt;**](SeoKeywordMonthlySearch.md) | Per-month search volume for the past 12 months (full view only). | [optional] 
**LastUpdatedAt** | **string** | When DataForSEO last refreshed the keyword metrics. | [optional] 
**Depth** | **int** | Search depth at which this keyword was found, relative to the seed keyword. | [optional] 
**RelatedKeywords** | **List&lt;string&gt;** | Keywords from the &#39;searches related to&#39; SERP element for this keyword. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

