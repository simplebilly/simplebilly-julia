# EmployeeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_employee**](EmployeeApi.md#create_employee) | **POST** /api/v1/employees | 
[**delete_employee**](EmployeeApi.md#delete_employee) | **DELETE** /api/v1/employees/{id} | 
[**employee_restore**](EmployeeApi.md#employee_restore) | **POST** /api/v1/employees/{id}/restore | 
[**get_employee**](EmployeeApi.md#get_employee) | **GET** /api/v1/employees/{id} | 
[**get_employee_payroll_summary**](EmployeeApi.md#get_employee_payroll_summary) | **GET** /api/v1/employees/{id}/payroll-summary | 
[**get_employees**](EmployeeApi.md#get_employees) | **GET** /api/v1/employees/ | 
[**update_employee**](EmployeeApi.md#update_employee) | **PUT** /api/v1/employees/{id} | 


# **create_employee**
> `create_employee`(_api::`EmployeeApi`, `employee_create`::`EmployeeCreate`; _mediaType=nothing) -> `Employee`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_employee`(_api::`EmployeeApi`, response_stream::`Channel`, `employee_create`::`EmployeeCreate`; _mediaType=nothing) -> `Channel`{ `Employee` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmployeeApi`** | API context | 
**`employee_create`** | [**`EmployeeCreate`**](EmployeeCreate.md) |  |

### Return type

[**`Employee`**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_employee**
> `delete_employee`(_api::`EmployeeApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_employee`(_api::`EmployeeApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmployeeApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **employee_restore**
> `employee_restore`(_api::`EmployeeApi`, `id`::`String`; _mediaType=nothing) -> `Employee`, `OpenAPI.Clients.ApiResponse` <br/>
> `employee_restore`(_api::`EmployeeApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Employee` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmployeeApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Employee`**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_employee**
> `get_employee`(_api::`EmployeeApi`, `id`::`String`; _mediaType=nothing) -> `Employee`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_employee`(_api::`EmployeeApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Employee` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmployeeApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

[**`Employee`**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_employee_payroll_summary**
> `get_employee_payroll_summary`(_api::`EmployeeApi`, `id`::`String`; `year`=nothing, _mediaType=nothing) -> `PayrollSummary`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_employee_payroll_summary`(_api::`EmployeeApi`, response_stream::`Channel`, `id`::`String`; `year`=nothing, _mediaType=nothing) -> `Channel`{ `PayrollSummary` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmployeeApi`** | API context | 
**`id`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** | Fiscal year for the breakdown; defaults to the current year. | [default to nothing]

### Return type

[**`PayrollSummary`**](PayrollSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_employees**
> `get_employees`(_api::`EmployeeApi`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Vector{Employee}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_employees`(_api::`EmployeeApi`, response_stream::`Channel`; `page`=nothing, `page_size`=nothing, `search`=nothing, `include_deleted`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{Employee}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmployeeApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`page`** | **`Int64`** |  | [default to nothing]
 **`page_size`** | **`Int64`** |  | [default to nothing]
 **`search`** | **`String`** |  | [default to nothing]
 **`include_deleted`** | **`Bool`** | Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [default to nothing]

### Return type

[**`Vector{Employee}`**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **update_employee**
> `update_employee`(_api::`EmployeeApi`, `id`::`String`, `employee_update`::`EmployeeUpdate`; _mediaType=nothing) -> `Employee`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_employee`(_api::`EmployeeApi`, response_stream::`Channel`, `id`::`String`, `employee_update`::`EmployeeUpdate`; _mediaType=nothing) -> `Channel`{ `Employee` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`EmployeeApi`** | API context | 
**`id`** | **`String`** |  |
**`employee_update`** | [**`EmployeeUpdate`**](EmployeeUpdate.md) |  |

### Return type

[**`Employee`**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

