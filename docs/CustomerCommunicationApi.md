# CustomerCommunicationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_communication**](CustomerCommunicationApi.md#create_communication) | **POST** /api/v1/communications | 
[**customercommunication_restore**](CustomerCommunicationApi.md#customercommunication_restore) | **POST** /api/v1/communications/{communication_id}/restore | 
[**delete_communication**](CustomerCommunicationApi.md#delete_communication) | **DELETE** /api/v1/communications/{communication_id} | 
[**get_communication**](CustomerCommunicationApi.md#get_communication) | **GET** /api/v1/communications/{communication_id} | 
[**get_contact_history**](CustomerCommunicationApi.md#get_contact_history) | **GET** /api/v1/contacts/{contact_id}/communications | 
[**list_communications**](CustomerCommunicationApi.md#list_communications) | **GET** /api/v1/communications/ | 
[**update_communication**](CustomerCommunicationApi.md#update_communication) | **PUT** /api/v1/communications/{communication_id} | 


# **create_communication**
> `create_communication`(_api::`CustomerCommunicationApi`, `customer_communication_create`::`CustomerCommunicationCreate`; _mediaType=nothing) -> `CustomerCommunication`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_communication`(_api::`CustomerCommunicationApi`, response_stream::`Channel`, `customer_communication_create`::`CustomerCommunicationCreate`; _mediaType=nothing) -> `Channel`{ `CustomerCommunication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerCommunicationApi`** | API context | 
**`customer_communication_create`** | [**`CustomerCommunicationCreate`**](CustomerCommunicationCreate.md) |  |

### Return type

[**`CustomerCommunication`**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **customercommunication_restore**
> `customercommunication_restore`(_api::`CustomerCommunicationApi`, `communication_id`::`String`; _mediaType=nothing) -> `CustomerCommunication`, `OpenAPI.Clients.ApiResponse` <br/>
> `customercommunication_restore`(_api::`CustomerCommunicationApi`, response_stream::`Channel`, `communication_id`::`String`; _mediaType=nothing) -> `Channel`{ `CustomerCommunication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerCommunicationApi`** | API context | 
**`communication_id`** | **`String`** |  |

### Return type

[**`CustomerCommunication`**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_communication**
> `delete_communication`(_api::`CustomerCommunicationApi`, `communication_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_communication`(_api::`CustomerCommunicationApi`, response_stream::`Channel`, `communication_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerCommunicationApi`** | API context | 
**`communication_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_communication**
> `get_communication`(_api::`CustomerCommunicationApi`, `communication_id`::`String`; _mediaType=nothing) -> `CustomerCommunication`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_communication`(_api::`CustomerCommunicationApi`, response_stream::`Channel`, `communication_id`::`String`; _mediaType=nothing) -> `Channel`{ `CustomerCommunication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerCommunicationApi`** | API context | 
**`communication_id`** | **`String`** |  |

### Return type

[**`CustomerCommunication`**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_contact_history**
> `get_contact_history`(_api::`CustomerCommunicationApi`, `contact_id`::`String`; _mediaType=nothing) -> `ContactHistoryResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_contact_history`(_api::`CustomerCommunicationApi`, response_stream::`Channel`, `contact_id`::`String`; _mediaType=nothing) -> `Channel`{ `ContactHistoryResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerCommunicationApi`** | API context | 
**`contact_id`** | **`String`** |  |

### Return type

[**`ContactHistoryResponse`**](ContactHistoryResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_communications**
> `list_communications`(_api::`CustomerCommunicationApi`; `page`=nothing, `page_size`=nothing, `contact_id`=nothing, `channel`=nothing, `direction`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Vector{CustomerCommunication}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_communications`(_api::`CustomerCommunicationApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `contact_id`=nothing, `channel`=nothing, `direction`=nothing, `from`=nothing, `to`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{CustomerCommunication}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerCommunicationApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`contact_id`** | **`String`** | Filter history to a single contact. | [default to nothing]
 **`channel`** | [**`CommunicationChannel`**](.md) |  | [default to nothing]
 **`direction`** | [**`CommunicationDirection`**](.md) |  | [default to nothing]
 **`from`** | **`Date`** | Only include communications after this ISO date (inclusive). | [default to nothing]
 **`to`** | **`Date`** | Only include communications before this ISO date (inclusive). | [default to nothing]

### Return type

[**`Vector{CustomerCommunication}`**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_communication**
> `update_communication`(_api::`CustomerCommunicationApi`, `communication_id`::`String`, `customer_communication_update`::`CustomerCommunicationUpdate`; _mediaType=nothing) -> `CustomerCommunication`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_communication`(_api::`CustomerCommunicationApi`, response_stream::`Channel`, `communication_id`::`String`, `customer_communication_update`::`CustomerCommunicationUpdate`; _mediaType=nothing) -> `Channel`{ `CustomerCommunication` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CustomerCommunicationApi`** | API context | 
**`communication_id`** | **`String`** |  |
**`customer_communication_update`** | [**`CustomerCommunicationUpdate`**](CustomerCommunicationUpdate.md) |  |

### Return type

[**`CustomerCommunication`**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

