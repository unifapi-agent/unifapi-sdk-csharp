# Unifapi.Sdk.Model.HotelSearchResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HotelIdentifier** | **string** | Unique hotel id. Pass it to /hotels/info for full details. | [optional] 
**Title** | **string** | Hotel or vacation rental name. | [optional] 
**Stars** | **int** | Hotel class rating, 1-5. | [optional] 
**IsPaid** | **bool** | True for paid hotel listings. | [optional] 
**Location** | [**HotelSearchGeo**](HotelSearchGeo.md) |  | [optional] 
**Reviews** | [**HotelSearchResultReviews**](HotelSearchResultReviews.md) |  | [optional] 
**Prices** | [**HotelSearchResultPrices**](HotelSearchResultPrices.md) |  | [optional] 
**OverviewImages** | **List&lt;string&gt;** | Preview image URLs for the hotel when present. | [optional] 
**IsBillable** | **bool** | Each hotel listing is one billable record. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

