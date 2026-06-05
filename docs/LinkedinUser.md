# Unifapi.Sdk.Model.LinkedinUser
Canonical LinkedIn user profile. `id` is the URL slug (`public_identifier`); `urn` is the LinkedIn internal opaque id required to call URN-keyed sub-resources source — gateway hides that detail behind `/linkedin/users/{id}/_*` (see ADR 0006).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | LinkedIn URL slug (public_identifier). Use this as the path parameter for every /linkedin/users/{id}/... endpoint. | 
**Urn** | **string** | LinkedIn internal URN (e.g. &#x60;ACoAA...&#x60;). Stable across username changes; required by certain LinkedIn-internal flows. | 
**Username** | **string** | Same value as &#x60;id&#x60;; included for cross-platform field parity. | 
**DisplayName** | **string** |  | 
**FirstName** | **string** |  | 
**LastName** | **string** |  | 
**Headline** | **string** |  | 
**AvatarUrl** | **string** |  | 
**CoverImageUrl** | **string** |  | 
**Location** | [**LinkedinLocation**](LinkedinLocation.md) |  | 
**IsPremium** | **bool** |  | 
**IsOpenToWork** | **bool** |  | 
**IsHiring** | **bool** |  | 
**IsCreator** | **bool** |  | 
**IsInfluencer** | **bool** |  | 
**IsTopVoice** | **bool** |  | 
**IsMemorialized** | **bool** |  | 
**CreatedAt** | **string** |  | 
**WebsiteUrl** | **string** |  | 
**AssociatedHashtags** | **List&lt;string&gt;** |  | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

