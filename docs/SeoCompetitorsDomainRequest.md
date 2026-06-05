# Unifapi.Sdk.Model.SeoCompetitorsDomainRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Target** | **string** | Target domain, such as example.com or https://example.com. Specified without www. | 
**Location** | [**SeoCompetitorsDomainLocation**](SeoCompetitorsDomainLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**ExcludeTopDomains** | **bool** | When true, exclude the largest global domains (e.g. wikipedia, amazon) from results. | [optional] 
**IntersectingDomains** | **List&lt;string&gt;** | Restrict results to competitors that also share keywords with these domains. | [optional] 
**Limit** | **int** | Maximum number of competing domains to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of domains to skip from the start of the results. | [optional] 
**View** | **SeoDomainMetricsView** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

