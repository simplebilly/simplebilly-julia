# BillingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_plans**](BillingApi.md#get_plans) | **GET** /api/v1/plans | All canonical plans (free/starter/business/enterprise) — the single source of truth lives in &#x60;crate::saasy::plans&#x60;, matching marketing.
[**get_quota_api**](BillingApi.md#get_quota_api) | **GET** /api/v1/quota | Effective limits + current usage for the calling tenant.
[**get_subscription_api**](BillingApi.md#get_subscription_api) | **GET** /api/v1/subscription | 
[**get_usage_api**](BillingApi.md#get_usage_api) | **GET** /api/v1/usage | 
[**paddle_subscription_webhook**](BillingApi.md#paddle_subscription_webhook) | **POST** /api/webhooks/paddle/subscription | Paddle Billing subscription webhook. Verifies the &#x60;Paddle-Signature&#x60; header (HMAC-SHA256 over &#x60;\&quot;{ts}:{raw_body}\&quot;&#x60; with the webhook secret), then updates &#x60;billing_info&#x60; and &#x60;tenants.plan&#x60; for the tenant identified by the subscription &#x60;custom_data&#x60; (JSON &#x60;{\&quot;tenant_id\&quot;: \&quot;...\&quot;}&#x60; or a bare tenant UUID).
[**put_quota_api**](BillingApi.md#put_quota_api) | **PUT** /api/v1/quota | Write the per-tenant quota override (&#x60;admin:settings&#x60;). An empty object clears the override.


# **get_plans**
> `get_plans`(_api::`BillingApi`; _mediaType=nothing) -> `ApiResponseVecPlan`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_plans`(_api::`BillingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ApiResponseVecPlan` }, `OpenAPI.Clients.ApiResponse`

All canonical plans (free/starter/business/enterprise) — the single source of truth lives in `crate::saasy::plans`, matching marketing.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ApiResponseVecPlan`**](ApiResponseVecPlan.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_quota_api**
> `get_quota_api`(_api::`BillingApi`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_quota_api`(_api::`BillingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Effective limits + current usage for the calling tenant.

### Required Parameters
This endpoint does not need any parameter.

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_subscription_api**
> `get_subscription_api`(_api::`BillingApi`; _mediaType=nothing) -> `ApiResponseSubscriptionOverview`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_subscription_api`(_api::`BillingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ApiResponseSubscriptionOverview` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ApiResponseSubscriptionOverview`**](ApiResponseSubscriptionOverview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_usage_api**
> `get_usage_api`(_api::`BillingApi`; `meter`=nothing, _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_usage_api`(_api::`BillingApi`, response_stream::`Channel`; `meter`=nothing, _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BillingApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`meter`** | **`String`** |  | [default to nothing]

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **paddle_subscription_webhook**
> `paddle_subscription_webhook`(_api::`BillingApi`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `paddle_subscription_webhook`(_api::`BillingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Paddle Billing subscription webhook. Verifies the `Paddle-Signature` header (HMAC-SHA256 over `\"{ts}:{raw_body}\"` with the webhook secret), then updates `billing_info` and `tenants.plan` for the tenant identified by the subscription `custom_data` (JSON `{\"tenant_id\": \"...\"}` or a bare tenant UUID).

### Required Parameters
This endpoint does not need any parameter.

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **put_quota_api**
> `put_quota_api`(_api::`BillingApi`, `quota_override`::`QuotaOverride`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `put_quota_api`(_api::`BillingApi`, response_stream::`Channel`, `quota_override`::`QuotaOverride`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Write the per-tenant quota override (`admin:settings`). An empty object clears the override.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BillingApi`** | API context | 
**`quota_override`** | [**`QuotaOverride`**](QuotaOverride.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

