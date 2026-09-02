# EventSubscriptionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_event_subscription**](EventSubscriptionApi.md#create_event_subscription) | **POST** /api/v1/event-subscriptions | 
[**delete_event_subscription**](EventSubscriptionApi.md#delete_event_subscription) | **DELETE** /api/v1/event-subscriptions/{subscription_id} | 
[**list_event_subscriptions**](EventSubscriptionApi.md#list_event_subscriptions) | **GET** /api/v1/event-subscriptions/ | 


# **create_event_subscription**
> `create_event_subscription`(_api::`EventSubscriptionApi`, `body`::`Any`; _mediaType=nothing) -> `EventSubscription`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_event_subscription`(_api::`EventSubscriptionApi`, response_stream::`Channel`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `EventSubscription` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EventSubscriptionApi`** | API context | 
**`body`** | **`Any`** |  |

### Return type

[**`EventSubscription`**](EventSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_event_subscription**
> `delete_event_subscription`(_api::`EventSubscriptionApi`, `subscription_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_event_subscription`(_api::`EventSubscriptionApi`, response_stream::`Channel`, `subscription_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EventSubscriptionApi`** | API context | 
**`subscription_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_event_subscriptions**
> `list_event_subscriptions`(_api::`EventSubscriptionApi`; _mediaType=nothing) -> `Vector{EventSubscription}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_event_subscriptions`(_api::`EventSubscriptionApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Vector{EventSubscription}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Vector{EventSubscription}`**](EventSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

