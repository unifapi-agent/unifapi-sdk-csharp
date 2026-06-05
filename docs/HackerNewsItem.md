# Unifapi.Sdk.Model.HackerNewsItem
Official Hacker News item. Stories, comments, jobs, polls, and poll options share this shape.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int** |  | 
**Deleted** | **bool** |  | [optional] 
**Type** | **HackerNewsItemType** |  | [optional] 
**By** | **string** |  | [optional] 
**Time** | **int** | Unix epoch seconds | [optional] 
**Text** | **string** | HTML text for comments, stories, polls, and jobs. | [optional] 
**Dead** | **bool** |  | [optional] 
**Parent** | **int** |  | [optional] 
**Poll** | **int** |  | [optional] 
**Kids** | **List&lt;int&gt;** |  | [optional] 
**Url** | **string** |  | [optional] 
**Score** | **int** |  | [optional] 
**Title** | **string** | HTML title for stories, polls, and jobs. | [optional] 
**Parts** | **List&lt;int&gt;** |  | [optional] 
**Descendants** | **int** |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

