# TicketMessageApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_messages_api**](TicketMessageApi.md#list_messages_api) | **GET** /api/v1/support/tickets/{ticket_id}/messages | 
[**send_message_api**](TicketMessageApi.md#send_message_api) | **POST** /api/v1/support/tickets/{ticket_id}/messages | 


# **list_messages_api**
> `list_messages_api`(_api::`TicketMessageApi`, `ticket_id`::`String`; _mediaType=nothing) -> `Vector{TicketMessage}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_messages_api`(_api::`TicketMessageApi`, response_stream::`Channel`, `ticket_id`::`String`; _mediaType=nothing) -> `Channel`{ `Vector{TicketMessage}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TicketMessageApi`** | API context | 
**`ticket_id`** | **`String`** |  |

### Return type

[**`Vector{TicketMessage}`**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **send_message_api**
> `send_message_api`(_api::`TicketMessageApi`, `ticket_id`::`String`, `send_message_dto`::`SendMessageDto`; _mediaType=nothing) -> `TicketMessage`, `OpenAPI.Clients.ApiResponse` <br/>
> `send_message_api`(_api::`TicketMessageApi`, response_stream::`Channel`, `ticket_id`::`String`, `send_message_dto`::`SendMessageDto`; _mediaType=nothing) -> `Channel`{ `TicketMessage` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TicketMessageApi`** | API context | 
**`ticket_id`** | **`String`** |  |
**`send_message_dto`** | [**`SendMessageDto`**](SendMessageDto.md) |  |

### Return type

[**`TicketMessage`**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

