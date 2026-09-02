# PayrollApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**payroll_approve**](PayrollApi.md#payroll_approve) | **POST** /api/v1/payroll/{id}/approve | 
[**payroll_autopay**](PayrollApi.md#payroll_autopay) | **POST** /api/v1/payroll/{id}/autopay | 
[**payroll_calculate**](PayrollApi.md#payroll_calculate) | **POST** /api/v1/payroll/{id}/calculate | 
[**payroll_create**](PayrollApi.md#payroll_create) | **POST** /api/v1/payroll | 
[**payroll_delete**](PayrollApi.md#payroll_delete) | **DELETE** /api/v1/payroll/{id} | 
[**payroll_elster_export**](PayrollApi.md#payroll_elster_export) | **POST** /api/v1/payroll/{id}/elster-export | 
[**payroll_email**](PayrollApi.md#payroll_email) | **POST** /api/v1/payroll/{id}/email | 
[**payroll_entry_pdf**](PayrollApi.md#payroll_entry_pdf) | **GET** /api/v1/payroll/{id}/entries/{entry_id}/pdf | 
[**payroll_get**](PayrollApi.md#payroll_get) | **GET** /api/v1/payroll/{id} | 
[**payroll_list**](PayrollApi.md#payroll_list) | **GET** /api/v1/payroll | 
[**payroll_pay**](PayrollApi.md#payroll_pay) | **POST** /api/v1/payroll/{id}/pay | 
[**payroll_pdf**](PayrollApi.md#payroll_pdf) | **GET** /api/v1/payroll/{id}/pdf | 
[**payroll_summary**](PayrollApi.md#payroll_summary) | **GET** /api/v1/payroll/summary/{year} | 
[**payroll_sv_meldungen**](PayrollApi.md#payroll_sv_meldungen) | **POST** /api/v1/payroll/{id}/sv-meldungen | 


# **payroll_approve**
> `payroll_approve`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `PayrollRunApi`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_approve`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `PayrollRunApi` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`PayrollRunApi`**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_autopay**
> `payroll_autopay`(_api::`PayrollApi`, `id`::`String`; `body`=nothing, _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_autopay`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; `body`=nothing, _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`body`** | **`Any`** |  | 

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_calculate**
> `payroll_calculate`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `PayrollRunApi`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_calculate`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `PayrollRunApi` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`PayrollRunApi`**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_create**
> `payroll_create`(_api::`PayrollApi`, `payroll_create_payload`::`PayrollCreatePayload`; _mediaType=nothing) -> `PayrollRunApi`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_create`(_api::`PayrollApi`, response_stream::`Channel`, `payroll_create_payload`::`PayrollCreatePayload`; _mediaType=nothing) -> `Channel`{ `PayrollRunApi` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`payroll_create_payload`** | [**`PayrollCreatePayload`**](PayrollCreatePayload.md) |  |

### Return type

[**`PayrollRunApi`**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_delete**
> `payroll_delete`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_delete`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_elster_export**
> `payroll_elster_export`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_elster_export`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_email**
> `payroll_email`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_email`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_entry_pdf**
> `payroll_entry_pdf`(_api::`PayrollApi`, `id`::`String`, `entry_id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_entry_pdf`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`, `entry_id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |
**`entry_id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_get**
> `payroll_get`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `PayrollRunApi`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_get`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `PayrollRunApi` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`PayrollRunApi`**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_list**
> `payroll_list`(_api::`PayrollApi`; `year`=nothing, `status`=nothing, _mediaType=nothing) -> `Vector{PayrollRunApi}`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_list`(_api::`PayrollApi`, response_stream::`Channel`; `year`=nothing, `status`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{PayrollRunApi}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`status`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{PayrollRunApi}`**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_pay**
> `payroll_pay`(_api::`PayrollApi`, `id`::`String`, `payroll_pay_payload`::`PayrollPayPayload`; _mediaType=nothing) -> `PayrollRunApi`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_pay`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`, `payroll_pay_payload`::`PayrollPayPayload`; _mediaType=nothing) -> `Channel`{ `PayrollRunApi` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |
**`payroll_pay_payload`** | [**`PayrollPayPayload`**](PayrollPayPayload.md) |  |

### Return type

[**`PayrollRunApi`**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_pdf**
> `payroll_pdf`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_pdf`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_summary**
> `payroll_summary`(_api::`PayrollApi`, `year`::`Int64`; _mediaType=nothing) -> `YearlyPayrollSummary`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_summary`(_api::`PayrollApi`, response_stream::`Channel`, `year`::`Int64`; _mediaType=nothing) -> `Channel`{ `YearlyPayrollSummary` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`year`** | **`Int64`** |  |

### Return type

[**`YearlyPayrollSummary`**](YearlyPayrollSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **payroll_sv_meldungen**
> `payroll_sv_meldungen`(_api::`PayrollApi`, `id`::`String`; _mediaType=nothing) -> `Any`, `OpenAPI.Clients.ApiResponse` <br/>
> `payroll_sv_meldungen`(_api::`PayrollApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Any` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`PayrollApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

**`Any`**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

