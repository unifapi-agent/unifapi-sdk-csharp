# Unifapi.Sdk.Model.BrowserScreenshotRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | Absolute http(s) URL of the page to render. | 
**WaitUntil** | **string** | When navigation is considered complete. &#x60;networkidle0&#x60; waits for the network to go idle (best for JavaScript-heavy pages); &#x60;load&#x60; is fastest. | [optional] 
**TimeoutMs** | **int** | Navigation timeout in milliseconds (1000–60000). | [optional] 
**Viewport** | [**BrowserScreenshotRequestViewport**](BrowserScreenshotRequestViewport.md) |  | [optional] 
**FullPage** | **bool** | Capture the full scrollable page instead of just the viewport. | [optional] 
**Format** | **string** | Output image format. | [optional] [default to FormatEnum.Png]
**Quality** | **int** | Compression quality (0–100). Only valid for &#x60;jpeg&#x60; and &#x60;webp&#x60;. | [optional] 
**Selector** | **string** | Capture only the first element matching this CSS selector. | [optional] 
**OmitBackground** | **bool** | Render a transparent background (ignored for &#x60;jpeg&#x60;). | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

