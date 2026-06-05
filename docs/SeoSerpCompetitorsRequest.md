# Unifapi.Sdk.Model.SeoSerpCompetitorsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Keywords** | **List&lt;string&gt;** | Seed keywords (1-200). Returns the domains that rank for them. | 
**Location** | [**SeoSerpCompetitorsLocation**](SeoSerpCompetitorsLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**IncludeSubdomains** | **bool** | When true (default), count subdomain rankings toward each domain. | [optional] 
**Limit** | **int** | Maximum number of competing domains to return. Defaults to 100. | [optional] 
**Offset** | **int** | Number of domains to skip from the start of the results. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

