# PackingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**complete_packing**](PackingApi.md#complete_packing) | **POST** /api/v1/packing/{order_number}/complete | Mark packing as complete and transition order to shipped
[**get_packing_queue**](PackingApi.md#get_packing_queue) | **GET** /api/v1/packing/queue | Get the packing queue - orders ready for packing
[**print_delivery_note**](PackingApi.md#print_delivery_note) | **POST** /api/v1/packing/{order_number}/print-delivery-note | Print delivery note (Lieferschein) for an order
[**print_label**](PackingApi.md#print_label) | **POST** /api/v1/packing/{order_number}/print-label | Print shipping label for an order
[**record_packing_video**](PackingApi.md#record_packing_video) | **POST** /api/v1/packing/{order_number}/record-video | Record video of packing process


# **complete_packing**
> `complete_packing`(_api::`PackingApi`, `order_number`::`String`, `packing_complete_request`::`PackingCompleteRequest`; _mediaType=nothing) -> `PackingCompleteResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `complete_packing`(_api::`PackingApi`, response_stream::`Channel`, `order_number`::`String`, `packing_complete_request`::`PackingCompleteRequest`; _mediaType=nothing) -> `Channel`{ `PackingCompleteResponse` }, `OpenAPI.Clients.ApiResponse`

Mark packing as complete and transition order to shipped

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PackingApi`** | API context | 
**`order_number`** | **`String`** |  |
**`packing_complete_request`** | [**`PackingCompleteRequest`**](PackingCompleteRequest.md) |  |

### Return type

[**`PackingCompleteResponse`**](PackingCompleteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_packing_queue**
> `get_packing_queue`(_api::`PackingApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, _mediaType=nothing) -> `PackingQueue`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_packing_queue`(_api::`PackingApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, _mediaType=nothing) -> `Channel`{ `PackingQueue` }, `OpenAPI.Clients.ApiResponse`

Get the packing queue - orders ready for packing

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PackingApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]

### Return type

[**`PackingQueue`**](PackingQueue.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **print_delivery_note**
> `print_delivery_note`(_api::`PackingApi`, `order_number`::`String`; _mediaType=nothing) -> `PrintDeliveryNoteResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `print_delivery_note`(_api::`PackingApi`, response_stream::`Channel`, `order_number`::`String`; _mediaType=nothing) -> `Channel`{ `PrintDeliveryNoteResponse` }, `OpenAPI.Clients.ApiResponse`

Print delivery note (Lieferschein) for an order

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PackingApi`** | API context | 
**`order_number`** | **`String`** |  |

### Return type

[**`PrintDeliveryNoteResponse`**](PrintDeliveryNoteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **print_label**
> `print_label`(_api::`PackingApi`, `order_number`::`String`; _mediaType=nothing) -> `PrintLabelResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `print_label`(_api::`PackingApi`, response_stream::`Channel`, `order_number`::`String`; _mediaType=nothing) -> `Channel`{ `PrintLabelResponse` }, `OpenAPI.Clients.ApiResponse`

Print shipping label for an order

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PackingApi`** | API context | 
**`order_number`** | **`String`** |  |

### Return type

[**`PrintLabelResponse`**](PrintLabelResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **record_packing_video**
> `record_packing_video`(_api::`PackingApi`, `order_number`::`String`, `body`::`Any`; _mediaType=nothing) -> `PackingVideoResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `record_packing_video`(_api::`PackingApi`, response_stream::`Channel`, `order_number`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `PackingVideoResponse` }, `OpenAPI.Clients.ApiResponse`

Record video of packing process

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PackingApi`** | API context | 
**`order_number`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`PackingVideoResponse`**](PackingVideoResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

