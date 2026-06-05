# Unifapi.Sdk.Model.Error

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | Closed vocabulary - see docs/adr/0003-error-model.md. | 
**Message** | **string** |  | 
**RequestId** | **string** | UnifAPI request id, e.g. &#x60;unif_&lt;id&gt;&#x60;. Source ids are not exposed. | [optional] 
**Issues** | **List&lt;Object&gt;** | Present only when type&#x3D;validation_error. | [optional] 
**Billing** | [**ErrorBilling**](ErrorBilling.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

