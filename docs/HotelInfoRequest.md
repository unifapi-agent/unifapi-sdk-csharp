# Unifapi.Sdk.Model.HotelInfoRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HotelIdentifier** | **string** | Unique hotel id returned by /hotels/search. | 
**Location** | [**HotelInfoLocation**](HotelInfoLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**CheckIn** | **string** | Check-in date. Date in YYYY-MM-DD format. | [optional] 
**CheckOut** | **string** | Check-out date. Date in YYYY-MM-DD format. | [optional] 
**Currency** | **string** | ISO 4217 currency code for prices, such as USD. | [optional] 
**Adults** | **int** | Number of adult guests. | [optional] 
**Children** | **List&lt;int&gt;** | Ages of children staying, used to refine availability and pricing. | [optional] 
**LoadPricesByDates** | **bool** | When true, return a daily price calendar across the requested date range instead of a single stay price. | [optional] 
**PricesStartDate** | **string** | Start date for the daily price calendar. Date in YYYY-MM-DD format. | [optional] 
**PricesEndDate** | **string** | End date for the daily price calendar. Date in YYYY-MM-DD format. | [optional] 
**PricesDateRange** | **string** | Predefined period for the daily price calendar, such as next_30_days. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

