# Unifapi.Sdk.Model.HotelSearchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Query** | **string** | Optional hotel name or search query. Combine with location to scope the search. | [optional] 
**Location** | [**HotelSearchLocation**](HotelSearchLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**Limit** | **int** | Number of hotels to return. Defaults to 10. | [optional] 
**CheckIn** | **string** | Check-in date. Date in YYYY-MM-DD format. | [optional] 
**CheckOut** | **string** | Check-out date. Date in YYYY-MM-DD format. | [optional] 
**Currency** | **string** | ISO 4217 currency code for prices, such as USD. | [optional] 
**Adults** | **int** | Number of adult guests. | [optional] 
**Children** | **List&lt;int&gt;** | Ages of children staying, used to refine availability and pricing. | [optional] 
**Stars** | **List&lt;int&gt;** | Filter to hotels with these class ratings, such as [4, 5]. | [optional] 
**MinRating** | **decimal** | Filter to hotels with at least this guest rating. | [optional] 
**SortBy** | **string** | Sort order for results. Defaults to relevance. | [optional] 
**MinPrice** | **int** | Minimum price per night. | [optional] 
**MaxPrice** | **int** | Maximum price per night. | [optional] 
**FreeCancellation** | **bool** | When true, only return hotels offering free cancellation. | [optional] 
**IsVacationRentals** | **bool** | When true, search vacation rentals instead of hotels. | [optional] 
**Amenities** | **List&lt;string&gt;** | Filter to hotels offering these amenities, such as pool or free_wifi. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

