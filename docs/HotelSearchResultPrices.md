# Unifapi.Sdk.Model.HotelSearchResultPrices

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Price** | **decimal** | Nightly price in the response currency. | [optional] 
**PriceWithoutDiscount** | **decimal** | Full nightly price before any discount, when a discount applies. | [optional] 
**Currency** | **string** | ISO 4217 currency code for the price, such as USD. | [optional] 
**DiscountText** | **string** | Discount label, such as \&quot;23% less than usual\&quot;. | [optional] 
**PricesByDates** | [**List&lt;HotelPriceByDate&gt;**](HotelPriceByDate.md) | Daily price calendar, populated when /hotels/info requests load_prices_by_dates. | [optional] 
**Extras** | **Dictionary** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

