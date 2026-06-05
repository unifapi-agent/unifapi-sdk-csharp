# Unifapi.Sdk.Model.InstagramPost

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Instagram URL slug (&#x60;shortcode&#x60;). Path parameter for /instagram/posts/{id}/... endpoints. | 
**Shortcode** | **string** |  | 
**MediaId** | **string** |  | 
**MediaType** | **decimal** | Source media_type: 1 &#x3D; image, 2 &#x3D; video, 8 &#x3D; carousel | 
**ProductType** | **string** | Source product_type: &#39;feed&#39; (image/photo), &#39;clips&#39; (reel), &#39;carousel_container&#39;, &#39;igtv&#39;, etc. | 
**TakenAt** | **decimal** | Unix-seconds timestamp. | 
**Caption** | **string** |  | 
**AccessibilityCaption** | **string** |  | 
**ImageUrl** | **string** | Largest available preview image (cover, for video/carousel). | 
**VideoUrl** | **string** | Highest-quality video URL when applicable; empty string otherwise. | 
**LikeCount** | **decimal** |  | 
**CommentCount** | **decimal** |  | 
**PlayCount** | **decimal** | Video plays. 0 for non-video media. | 
**ViewCount** | **decimal** | Reel/video views (separate from plays on IG side). 0 when N/A. | 
**IsPaidPartnership** | **bool** |  | 
**HasAudio** | **bool** |  | 
**CarouselCount** | **decimal** | Number of carousel items, or 0 if not a carousel. | 
**Carousel** | [**List&lt;InstagramCarouselItem&gt;**](InstagramCarouselItem.md) | Carousel items when media_type &#x3D;&#x3D;&#x3D; 8; empty array otherwise. | 
**User** | [**InstagramUserPreview**](InstagramUserPreview.md) |  | 
**Location** | [**InstagramLocationLite**](InstagramLocationLite.md) |  | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

