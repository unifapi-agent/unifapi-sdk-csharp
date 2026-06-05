# Unifapi.Sdk.Model.LinkedinCompany

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | URL slug (LinkedIn&#39;s &#x60;universal_name&#x60;). Use this for every /linkedin/companies/{id}/... endpoint. | 
**CompanyId** | **string** | Numeric LinkedIn-internal id. Exposed because LinkedIn pages and ad-library URLs reference it; not needed for any /linkedin/_* call. | 
**Name** | **string** |  | 
**Description** | **string** |  | 
**WebsiteUrl** | **string** |  | 
**LinkedinUrl** | **string** |  | 
**IsVerified** | **bool** |  | 
**IsActive** | **bool** |  | 
**FollowerCount** | **int** |  | 
**EmployeeCount** | **int** |  | 
**EmployeeCountRange** | [**LinkedinEmployeeCountRange**](LinkedinEmployeeCountRange.md) |  | 
**Industries** | **List&lt;string&gt;** |  | 
**Specialities** | **List&lt;string&gt;** |  | 
**Headquarters** | [**LinkedinHeadquarters**](LinkedinHeadquarters.md) |  | 
**LogoUrl** | **string** |  | 
**CoverImageUrl** | **string** |  | 
**Hashtags** | [**List&lt;LinkedinCompanyHashtagsInner&gt;**](LinkedinCompanyHashtagsInner.md) |  | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

