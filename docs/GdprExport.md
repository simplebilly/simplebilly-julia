# GdprExport


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`activityLog`** | [**`Vector{GdprActivity}`**](GdprActivity.md) |  | [default to nothing]
**`apiKeys`** | [**`Vector{GdprApiKey}`**](GdprApiKey.md) | Key identifiers and names only — never a usable credential. | [default to nothing]
**`billing`** | [**`Vector{GdprBillingInfo}`**](GdprBillingInfo.md) |  | [default to nothing]
**`exportedAt`** | **`ZonedDateTime`** |  | [default to nothing]
**`generatedByAi`** | **`Bool`** | Honesty field: this document is a plain data dump, never AI-generated. | [default to nothing]
**`notifications`** | [**`Vector{GdprNotification}`**](GdprNotification.md) |  | [default to nothing]
**`refreshTokens`** | [**`Vector{GdprRefreshToken}`**](GdprRefreshToken.md) | Session records: metadata only, never the token hash. | [default to nothing]
**`tenants`** | [**`Vector{GdprTenant}`**](GdprTenant.md) |  | [default to nothing]
**`usageEvents`** | [**`Vector{GdprUsageEvent}`**](GdprUsageEvent.md) |  | [default to nothing]
**`user`** | [**`*GdprUser`**](GdprUser.md) |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


