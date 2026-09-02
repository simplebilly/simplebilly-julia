# ApiResponseSubscriptionOverviewData


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`currentPeriodEnd`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`features`** | [**`*PlanFeatures`**](PlanFeatures.md) |  | [default to nothing]
**`isTrialing`** | **`Bool`** |  | [default to nothing]
**`limits`** | [**`*PlanLimits`**](PlanLimits.md) |  | [default to nothing]
**`manageUrl`** | **`String`** |  | [optional] [default to nothing]
**`plan`** | **`String`** | Resolved plan id (free/starter/business/enterprise, or a custom override id). | [default to nothing]
**`planName`** | **`String`** |  | [default to nothing]
**`priceEur`** | **`Float64`** | Monthly price in EUR; &#x60;-1.0&#x60; &#x3D; custom pricing (enterprise). | [default to nothing]
**`quantity`** | **`Int64`** |  | [optional] [default to nothing]
**`status`** | **`String`** |  | [optional] [default to nothing]
**`subscriptionId`** | **`String`** |  | [optional] [default to nothing]
**`trialEndsAt`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`usage`** | [**`*UsageSnapshot`**](UsageSnapshot.md) |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


