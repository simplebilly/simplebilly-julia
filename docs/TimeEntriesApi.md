# TimeEntriesApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**clock_in_time_entry**](TimeEntriesApi.md#clock_in_time_entry) | **POST** /api/v1/time-entries | Clock in for the authenticated user (resolved via their employee profile).
[**clock_out_time_entry**](TimeEntriesApi.md#clock_out_time_entry) | **PATCH** /api/v1/time-entries/{id} | Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.
[**get_labor_costs**](TimeEntriesApi.md#get_labor_costs) | **GET** /api/v1/labor-costs | Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate.
[**list_time_entries**](TimeEntriesApi.md#list_time_entries) | **GET** /api/v1/time-entries | List time entries with optional date-range / active / employee filters.


# **clock_in_time_entry**
> `clock_in_time_entry`(_api::`TimeEntriesApi`, `time_entry_clock_in`::`TimeEntryClockIn`; _mediaType=nothing) -> `TimeEntryDto`, `OpenAPI.Clients.ApiResponse` <br/>
> `clock_in_time_entry`(_api::`TimeEntriesApi`, response_stream::`Channel`, `time_entry_clock_in`::`TimeEntryClockIn`; _mediaType=nothing) -> `Channel`{ `TimeEntryDto` }, `OpenAPI.Clients.ApiResponse`

Clock in for the authenticated user (resolved via their employee profile).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TimeEntriesApi`** | API context | 
**`time_entry_clock_in`** | [**`TimeEntryClockIn`**](TimeEntryClockIn.md) |  |

### Return type

[**`TimeEntryDto`**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **clock_out_time_entry**
> `clock_out_time_entry`(_api::`TimeEntriesApi`, `id`::`String`, `time_entry_clock_out`::`TimeEntryClockOut`; _mediaType=nothing) -> `TimeEntryDto`, `OpenAPI.Clients.ApiResponse` <br/>
> `clock_out_time_entry`(_api::`TimeEntriesApi`, response_stream::`Channel`, `id`::`String`, `time_entry_clock_out`::`TimeEntryClockOut`; _mediaType=nothing) -> `Channel`{ `TimeEntryDto` }, `OpenAPI.Clients.ApiResponse`

Clock out an entry: the entry's owner, or anyone with `time_entries:write`.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TimeEntriesApi`** | API context | 
**`id`** | **`String`** |  |
**`time_entry_clock_out`** | [**`TimeEntryClockOut`**](TimeEntryClockOut.md) |  |

### Return type

[**`TimeEntryDto`**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_labor_costs**
> `get_labor_costs`(_api::`TimeEntriesApi`, `from`::`Date`, `to`::`Date`, `group_by`::`String`; _mediaType=nothing) -> `Vector{LaborCostRow}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_labor_costs`(_api::`TimeEntriesApi`, response_stream::`Channel`, `from`::`Date`, `to`::`Date`, `group_by`::`String`; _mediaType=nothing) -> `Channel`{ `Vector{LaborCostRow}` }, `OpenAPI.Clients.ApiResponse`

Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee's hourly cost rate.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TimeEntriesApi`** | API context | 
**`from`** | **`Date`** |  |
**`to`** | **`Date`** |  |
**`group_by`** | **`String`** | One of \&quot;employee\&quot;, \&quot;order\&quot; or \&quot;day\&quot;. |

### Return type

[**`Vector{LaborCostRow}`**](LaborCostRow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_time_entries**
> `list_time_entries`(_api::`TimeEntriesApi`; `from`=nothing, `to`=nothing, `active`=nothing, `employee_id`=nothing, _mediaType=nothing) -> `Vector{TimeEntryDto}`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_time_entries`(_api::`TimeEntriesApi`, response_stream::`Channel`; `from`=nothing, `to`=nothing, `active`=nothing, `employee_id`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{TimeEntryDto}` }, `OpenAPI.Clients.ApiResponse`

List time entries with optional date-range / active / employee filters.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TimeEntriesApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`from`** | **`Date`** |  | [default to nothing]
 **`to`** | **`Date`** |  | [default to nothing]
 **`active`** | **`Bool`** | Only currently running shifts (clock_in set, clock_out null). | [default to nothing]
 **`employee_id`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{TimeEntryDto}`**](TimeEntryDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

