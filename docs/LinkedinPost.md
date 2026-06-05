# Unifapi.Sdk.Model.LinkedinPost

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ShareUrn** | **string** |  | 
**PostType** | **string** | ugc | activity | share | ... | 
**Text** | **string** |  | 
**Url** | **string** |  | 
**CreateTime** | **int** | Unix epoch seconds | 
**CreatedAt** | **string** | Original ISO timestamp | 
**LikeCount** | **int** |  | 
**CommentCount** | **int** |  | 
**ShareCount** | **int** |  | 
**Reactions** | [**List&lt;LinkedinPostReactionsInner&gt;**](LinkedinPostReactionsInner.md) |  | 
**Author** | [**LinkedinPostAuthor**](LinkedinPostAuthor.md) |  | 
**Content** | **Dictionary&lt;string, Object&gt;** | Pass-through LinkedIn post body block (images, video, document, article, celebration, poll, event). LinkedIn&#39;s structure for each is complex and evolving — kept as-is rather than reshaped. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

