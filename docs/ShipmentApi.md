# ShipmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipment**](ShipmentApi.md#create_shipment) | **POST** /api/v1/shipments | 
[**create_shipment_from_order**](ShipmentApi.md#create_shipment_from_order) | **POST** /api/v1/orders/{order_number}/shipments | Create a real shipment for an order: calls the configured carrier&#39;s label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped.
[**delete_shipment**](ShipmentApi.md#delete_shipment) | **DELETE** /api/v1/shipments/{shipment_id} | 
[**get_shipment**](ShipmentApi.md#get_shipment) | **GET** /api/v1/shipments/{shipment_id} | 
[**list_shipments**](ShipmentApi.md#list_shipments) | **GET** /api/v1/shipments | 
[**track_order_public**](ShipmentApi.md#track_order_public) | **POST** /api/v1/public/track | Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API).
[**track_shipment_api**](ShipmentApi.md#track_shipment_api) | **GET** /api/v1/shipments/{shipment_id}/tracking | 
[**update_shipment_status**](ShipmentApi.md#update_shipment_status) | **PUT** /api/v1/shipments/{shipment_id}/status | 


# **create_shipment**
> `create_shipment`(_api::`ShipmentApi`, `shipment`::`Shipment`; _mediaType=nothing) -> `Shipment`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_shipment`(_api::`ShipmentApi`, response_stream::`Channel`, `shipment`::`Shipment`; _mediaType=nothing) -> `Channel`{ `Shipment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 
**`shipment`** | [**`Shipment`**](Shipment.md) |  |

### Return type

[**`Shipment`**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **create_shipment_from_order**
> `create_shipment_from_order`(_api::`ShipmentApi`, `order_number`::`String`, `create_shipment_request`::`CreateShipmentRequest`; _mediaType=nothing) -> `Shipment`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_shipment_from_order`(_api::`ShipmentApi`, response_stream::`Channel`, `order_number`::`String`, `create_shipment_request`::`CreateShipmentRequest`; _mediaType=nothing) -> `Channel`{ `Shipment` }, `OpenAPI.Clients.ApiResponse`

Create a real shipment for an order: calls the configured carrier's label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 
**`order_number`** | **`String`** |  |
**`create_shipment_request`** | [**`CreateShipmentRequest`**](CreateShipmentRequest.md) |  |

### Return type

[**`Shipment`**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_shipment**
> `delete_shipment`(_api::`ShipmentApi`, `shipment_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_shipment`(_api::`ShipmentApi`, response_stream::`Channel`, `shipment_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 
**`shipment_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_shipment**
> `get_shipment`(_api::`ShipmentApi`, `shipment_id`::`String`; _mediaType=nothing) -> `Shipment`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_shipment`(_api::`ShipmentApi`, response_stream::`Channel`, `shipment_id`::`String`; _mediaType=nothing) -> `Channel`{ `Shipment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 
**`shipment_id`** | **`String`** |  |

### Return type

[**`Shipment`**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_shipments**
> `list_shipments`(_api::`ShipmentApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Shipment}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_shipments`(_api::`ShipmentApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Shipment}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Shipment}`**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **track_order_public**
> `track_order_public`(_api::`ShipmentApi`, `track_order_request`::`TrackOrderRequest`; _mediaType=nothing) -> `TrackOrderResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `track_order_public`(_api::`ShipmentApi`, response_stream::`Channel`, `track_order_request`::`TrackOrderRequest`; _mediaType=nothing) -> `Channel`{ `TrackOrderResponse` }, `OpenAPI.Clients.ApiResponse`

Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 
**`track_order_request`** | [**`TrackOrderRequest`**](TrackOrderRequest.md) |  |

### Return type

[**`TrackOrderResponse`**](TrackOrderResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **track_shipment_api**
> `track_shipment_api`(_api::`ShipmentApi`, `shipment_id`::`String`; _mediaType=nothing) -> `TrackingInfo`, `OpenAPI.Clients.ApiResponse` <br/>
> `track_shipment_api`(_api::`ShipmentApi`, response_stream::`Channel`, `shipment_id`::`String`; _mediaType=nothing) -> `Channel`{ `TrackingInfo` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 
**`shipment_id`** | **`String`** |  |

### Return type

[**`TrackingInfo`**](TrackingInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_shipment_status**
> `update_shipment_status`(_api::`ShipmentApi`, `shipment_id`::`String`, `shipment_status_update`::`ShipmentStatusUpdate`; _mediaType=nothing) -> `Shipment`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_shipment_status`(_api::`ShipmentApi`, response_stream::`Channel`, `shipment_id`::`String`, `shipment_status_update`::`ShipmentStatusUpdate`; _mediaType=nothing) -> `Channel`{ `Shipment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`ShipmentApi`** | API context | 
**`shipment_id`** | **`String`** |  |
**`shipment_status_update`** | [**`ShipmentStatusUpdate`**](ShipmentStatusUpdate.md) |  |

### Return type

[**`Shipment`**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

