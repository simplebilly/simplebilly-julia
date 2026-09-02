# DeliveryAppointmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_delivery_appointment**](DeliveryAppointmentApi.md#create_delivery_appointment) | **POST** /api/v1/delivery-appointments | 
[**delete_delivery_appointment**](DeliveryAppointmentApi.md#delete_delivery_appointment) | **DELETE** /api/v1/delivery-appointments/{appointment_id} | 
[**get_delivery_appointment**](DeliveryAppointmentApi.md#get_delivery_appointment) | **GET** /api/v1/delivery-appointments/{appointment_id} | 
[**get_public_delivery_appointment_status**](DeliveryAppointmentApi.md#get_public_delivery_appointment_status) | **GET** /api/v1/public/delivery-appointments/status | Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.
[**list_delivery_appointments**](DeliveryAppointmentApi.md#list_delivery_appointments) | **GET** /api/v1/delivery-appointments | 
[**request_public_delivery_appointment**](DeliveryAppointmentApi.md#request_public_delivery_appointment) | **POST** /api/v1/public/delivery-appointments/request | Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.
[**update_delivery_appointment**](DeliveryAppointmentApi.md#update_delivery_appointment) | **PUT** /api/v1/delivery-appointments/{appointment_id} | 
[**update_delivery_appointment_status**](DeliveryAppointmentApi.md#update_delivery_appointment_status) | **PUT** /api/v1/delivery-appointments/{appointment_id}/status | 


# **create_delivery_appointment**
> `create_delivery_appointment`(_api::`DeliveryAppointmentApi`, `delivery_appointment_create`::`DeliveryAppointmentCreate`; _mediaType=nothing) -> `DeliveryAppointment`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_delivery_appointment`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`, `delivery_appointment_create`::`DeliveryAppointmentCreate`; _mediaType=nothing) -> `Channel`{ `DeliveryAppointment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 
**`delivery_appointment_create`** | [**`DeliveryAppointmentCreate`**](DeliveryAppointmentCreate.md) |  |

### Return type

[**`DeliveryAppointment`**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_delivery_appointment**
> `delete_delivery_appointment`(_api::`DeliveryAppointmentApi`, `appointment_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_delivery_appointment`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`, `appointment_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 
**`appointment_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_delivery_appointment**
> `get_delivery_appointment`(_api::`DeliveryAppointmentApi`, `appointment_id`::`String`; _mediaType=nothing) -> `DeliveryAppointment`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_delivery_appointment`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`, `appointment_id`::`String`; _mediaType=nothing) -> `Channel`{ `DeliveryAppointment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 
**`appointment_id`** | **`String`** |  |

### Return type

[**`DeliveryAppointment`**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_public_delivery_appointment_status**
> `get_public_delivery_appointment_status`(_api::`DeliveryAppointmentApi`, `appointment_id`::`String`, `email`::`String`, `token`::`String`; _mediaType=nothing) -> `PublicDeliveryAppointmentStatusResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_public_delivery_appointment_status`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`, `appointment_id`::`String`, `email`::`String`, `token`::`String`; _mediaType=nothing) -> `Channel`{ `PublicDeliveryAppointmentStatusResponse` }, `OpenAPI.Clients.ApiResponse`

Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 
**`appointment_id`** | **`String`** |  |
**`email`** | **`String`** |  |
**`token`** | **`String`** |  |

### Return type

[**`PublicDeliveryAppointmentStatusResponse`**](PublicDeliveryAppointmentStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_delivery_appointments**
> `list_delivery_appointments`(_api::`DeliveryAppointmentApi`; `page`=nothing, `page_size`=nothing, `status`=nothing, `warehouse_id`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Vector{DeliveryAppointment}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_delivery_appointments`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `status`=nothing, `warehouse_id`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{DeliveryAppointment}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]
 **`warehouse_id`** | **`String`** |  | [default to nothing]
 **`from`** | **`Date`** |  | [default to nothing]
 **`to`** | **`Date`** |  | [default to nothing]

### Return type

[**`Vector{DeliveryAppointment}`**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **request_public_delivery_appointment**
> `request_public_delivery_appointment`(_api::`DeliveryAppointmentApi`, `public_delivery_appointment_request`::`PublicDeliveryAppointmentRequest`; _mediaType=nothing) -> `PublicDeliveryAppointmentResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `request_public_delivery_appointment`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`, `public_delivery_appointment_request`::`PublicDeliveryAppointmentRequest`; _mediaType=nothing) -> `Channel`{ `PublicDeliveryAppointmentResponse` }, `OpenAPI.Clients.ApiResponse`

Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by `code` — never from the request.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 
**`public_delivery_appointment_request`** | [**`PublicDeliveryAppointmentRequest`**](PublicDeliveryAppointmentRequest.md) |  |

### Return type

[**`PublicDeliveryAppointmentResponse`**](PublicDeliveryAppointmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_delivery_appointment**
> `update_delivery_appointment`(_api::`DeliveryAppointmentApi`, `appointment_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `DeliveryAppointment`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_delivery_appointment`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`, `appointment_id`::`String`, `body`::`Any`; _mediaType=nothing) -> `Channel`{ `DeliveryAppointment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 
**`appointment_id`** | **`String`** |  |
**`body`** | **`Any`** |  |

### Return type

[**`DeliveryAppointment`**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_delivery_appointment_status**
> `update_delivery_appointment_status`(_api::`DeliveryAppointmentApi`, `appointment_id`::`String`, `appointment_status_update`::`AppointmentStatusUpdate`; _mediaType=nothing) -> `DeliveryAppointment`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_delivery_appointment_status`(_api::`DeliveryAppointmentApi`, response_stream::`Channel`, `appointment_id`::`String`, `appointment_status_update`::`AppointmentStatusUpdate`; _mediaType=nothing) -> `Channel`{ `DeliveryAppointment` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`DeliveryAppointmentApi`** | API context | 
**`appointment_id`** | **`String`** |  |
**`appointment_status_update`** | [**`AppointmentStatusUpdate`**](AppointmentStatusUpdate.md) |  |

### Return type

[**`DeliveryAppointment`**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

