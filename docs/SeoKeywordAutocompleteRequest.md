# Unifapi.Sdk.Model.SeoKeywordAutocompleteRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Keyword** | **string** | Seed query typed into Google search. Returns the autocomplete suggestions Google offers. | 
**Location** | [**SeoAutocompleteLocation**](SeoAutocompleteLocation.md) |  | [optional] 
**Language** | **string** | Search language as an ISO code or full language name. Defaults to en. | [optional] 
**CursorPointer** | **int** | Cursor position within the keyword. Defaults to the end of the keyword, matching how Google expands suggestions as you type. | [optional] 
**VarClient** | **string** | Autocomplete client to emulate, such as chrome or gws-wiz. Different clients can return different suggestion sets. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

