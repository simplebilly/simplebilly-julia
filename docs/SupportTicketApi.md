# SupportTicketApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_ticket_api**](SupportTicketApi.md#create_ticket_api) | **POST** /api/v1/support/tickets | 
[**delete_ticket_api**](SupportTicketApi.md#delete_ticket_api) | **DELETE** /api/v1/support/tickets/{ticket_id} | 
[**get_ticket_api**](SupportTicketApi.md#get_ticket_api) | **GET** /api/v1/support/tickets/{ticket_id} | 
[**list_tickets_api**](SupportTicketApi.md#list_tickets_api) | **GET** /api/v1/support/tickets | 
[**update_ticket_api**](SupportTicketApi.md#update_ticket_api) | **PUT** /api/v1/support/tickets/{ticket_id} | 


# **create_ticket_api**
> `create_ticket_api`(_api::`SupportTicketApi`, `create_ticket_request`::`CreateTicketRequest`; _mediaType=nothing) -> `SupportTicket`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_ticket_api`(_api::`SupportTicketApi`, response_stream::`Channel`, `create_ticket_request`::`CreateTicketRequest`; _mediaType=nothing) -> `Channel`{ `SupportTicket` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportTicketApi`** | API context | 
**`create_ticket_request`** | [**`CreateTicketRequest`**](CreateTicketRequest.md) |  |

### Return type

[**`SupportTicket`**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_ticket_api**
> `delete_ticket_api`(_api::`SupportTicketApi`, `ticket_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_ticket_api`(_api::`SupportTicketApi`, response_stream::`Channel`, `ticket_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportTicketApi`** | API context | 
**`ticket_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_ticket_api**
> `get_ticket_api`(_api::`SupportTicketApi`, `ticket_id`::`String`; _mediaType=nothing) -> `SupportTicket`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_ticket_api`(_api::`SupportTicketApi`, response_stream::`Channel`, `ticket_id`::`String`; _mediaType=nothing) -> `Channel`{ `SupportTicket` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportTicketApi`** | API context | 
**`ticket_id`** | **`String`** |  |

### Return type

[**`SupportTicket`**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_tickets_api**
> `list_tickets_api`(_api::`SupportTicketApi`; `status`=nothing, `priority`=nothing, `assigned_to`=nothing, `channel_type`=nothing, `customer_id`=nothing, `search`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Vector{SupportTicket}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_tickets_api`(_api::`SupportTicketApi`, response_stream::`Channel`; `status`=nothing, `priority`=nothing, `assigned_to`=nothing, `channel_type`=nothing, `customer_id`=nothing, `search`=nothing, `page`=nothing, `page_size`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{SupportTicket}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportTicketApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`status`** | **`String`** |  | [default to nothing]
 **`priority`** | **`String`** |  | [default to nothing]
 **`assigned_to`** | **`String`** |  | [default to nothing]
 **`channel_type`** | **`String`** |  | [default to nothing]
 **`customer_id`** | **`String`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]

### Return type

[**`Vector{SupportTicket}`**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_ticket_api**
> `update_ticket_api`(_api::`SupportTicketApi`, `ticket_id`::`String`, `support_ticket_update`::`SupportTicketUpdate`; _mediaType=nothing) -> `SupportTicket`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_ticket_api`(_api::`SupportTicketApi`, response_stream::`Channel`, `ticket_id`::`String`, `support_ticket_update`::`SupportTicketUpdate`; _mediaType=nothing) -> `Channel`{ `SupportTicket` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`SupportTicketApi`** | API context | 
**`ticket_id`** | **`String`** |  |
**`support_ticket_update`** | [**`SupportTicketUpdate`**](SupportTicketUpdate.md) |  |

### Return type

[**`SupportTicket`**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

