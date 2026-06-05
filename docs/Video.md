# Unifapi.Sdk.Model.Video
A canonical TikTok video. Counts (`like_count`, etc.) are source snapshots and not guaranteed monotonic.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Title** | **string** | Per ADR 0004 Rule 6: TikTok title is the video description. | 
**VideoDescription** | **string** |  | 
**CreateTime** | **int** | Unix epoch seconds | 
**Duration** | **decimal** | Seconds | 
**CoverImageUrl** | **string** |  | 
**ShareUrl** | **string** | Tracking-param-stripped canonical URL | 
**EmbedLink** | **string** |  | 
**Width** | **int** |  | 
**Height** | **int** |  | 
**LikeCount** | **int** |  | 
**CommentCount** | **int** |  | 
**ShareCount** | **int** |  | 
**ViewCount** | **int** |  | 
**Author** | [**Author**](Author.md) |  | 
**Region** | **string** |  | 
**Hashtags** | **List&lt;string&gt;** |  | 
**Music** | [**Music**](Music.md) |  | 
**IsImagePost** | **bool** |  | 
**PlayUrl** | **string** |  | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

