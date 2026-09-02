# WebhooksApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_subscription**](WebhooksApi.md#create_subscription) | **POST** /api/v1/webhook-subscriptions | Create a webhook subscription (outbound hook).
[**delete_subscription**](WebhooksApi.md#delete_subscription) | **DELETE** /api/v1/webhook-subscriptions/{subscription_id} | Delete a webhook subscription.
[**emit_api**](WebhooksApi.md#emit_api) | **POST** /api/v1/webhooks/emit | Manually fire an event against matching hooks (for testing/flows).
[**list_event**](WebhooksApi.md#list_event) | **GET** /api/v1/webhook-events | List webhook events (inbound + outbound log).
[**list_subscriptions**](WebhooksApi.md#list_subscriptions) | **GET** /api/v1/webhook-subscriptions | List webhook subscriptions for the tenant.
[**update_subscription**](WebhooksApi.md#update_subscription) | **PUT** /api/v1/webhook-subscriptions/{subscription_id} | Update a webhook subscription.


# **create_subscription**
> `create_subscription`(_api::`WebhooksApi`, `create_subscription_request`::`CreateSubscriptionRequest`; _mediaType=nothing) -> `WebhookSubscription`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_subscription`(_api::`WebhooksApi`, response_stream::`Channel`, `create_subscription_request`::`CreateSubscriptionRequest`; _mediaType=nothing) -> `Channel`{ `WebhookSubscription` }, `OpenAPI.Clients.ApiResponse`

Create a webhook subscription (outbound hook).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WebhooksApi`** | API context | 
**`create_subscription_request`** | [**`CreateSubscriptionRequest`**](CreateSubscriptionRequest.md) |  |

### Return type

[**`WebhookSubscription`**](WebhookSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_subscription**
> `delete_subscription`(_api::`WebhooksApi`, `subscription_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_subscription`(_api::`WebhooksApi`, response_stream::`Channel`, `subscription_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Delete a webhook subscription.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WebhooksApi`** | API context | 
**`subscription_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **emit_api**
> `emit_api`(_api::`WebhooksApi`, `emit_event_request`::`EmitEventRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `emit_api`(_api::`WebhooksApi`, response_stream::`Channel`, `emit_event_request`::`EmitEventRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Manually fire an event against matching hooks (for testing/flows).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WebhooksApi`** | API context | 
**`emit_event_request`** | [**`EmitEventRequest`**](EmitEventRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_event**
> `list_event`(_api::`WebhooksApi`; _mediaType=nothing) -> `Vector{WebhookEvent}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_event`(_api::`WebhooksApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{WebhookEvent}` }, `OpenAPI.Clients.ApiResponse`

List webhook events (inbound + outbound log).

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{WebhookEvent}`**](WebhookEvent.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_subscriptions**
> `list_subscriptions`(_api::`WebhooksApi`; _mediaType=nothing) -> `Vector{WebhookSubscription}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_subscriptions`(_api::`WebhooksApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{WebhookSubscription}` }, `OpenAPI.Clients.ApiResponse`

List webhook subscriptions for the tenant.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{WebhookSubscription}`**](WebhookSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_subscription**
> `update_subscription`(_api::`WebhooksApi`, `subscription_id`::`String`, `update_subscription_request`::`UpdateSubscriptionRequest`; _mediaType=nothing) -> `WebhookSubscription`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_subscription`(_api::`WebhooksApi`, response_stream::`Channel`, `subscription_id`::`String`, `update_subscription_request`::`UpdateSubscriptionRequest`; _mediaType=nothing) -> `Channel`{ `WebhookSubscription` }, `OpenAPI.Clients.ApiResponse`

Update a webhook subscription.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`WebhooksApi`** | API context | 
**`subscription_id`** | **`String`** |  |
**`update_subscription_request`** | [**`UpdateSubscriptionRequest`**](UpdateSubscriptionRequest.md) |  |

### Return type

[**`WebhookSubscription`**](WebhookSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

