# BookkeepingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allocate_payment_api**](BookkeepingApi.md#allocate_payment_api) | **POST** /api/v1/payments/allocate | Allocate a payment to an invoice
[**bwa_report_api**](BookkeepingApi.md#bwa_report_api) | **GET** /api/v1/bookkeeping/bwa | Get BWA (Betriebswirtschaftliche Auswertung) report
[**elster_status_api**](BookkeepingApi.md#elster_status_api) | **GET** /api/v1/bookkeeping/elster/status | 
[**elster_validate_api**](BookkeepingApi.md#elster_validate_api) | **POST** /api/v1/bookkeeping/ustva/elster-validate | 
[**elster_xml_api**](BookkeepingApi.md#elster_xml_api) | **GET** /api/v1/bookkeeping/ustva/elster-xml | 
[**get_cashflow**](BookkeepingApi.md#get_cashflow) | **GET** /api/v1/bookkeeping/cashflow | GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.
[**get_liquidity**](BookkeepingApi.md#get_liquidity) | **GET** /api/v1/bookkeeping/liquidity | GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.
[**get_open_invoices_api**](BookkeepingApi.md#get_open_invoices_api) | **GET** /api/v1/payments/open-invoices/{customer_id} | Get open invoices for a customer
[**get_verfahrensdokumentation**](BookkeepingApi.md#get_verfahrensdokumentation) | **GET** /api/v1/bookkeeping/verfahrensdokumentation | GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.
[**run_dunning_api**](BookkeepingApi.md#run_dunning_api) | **POST** /api/v1/bookkeeping/dunning | 


# **allocate_payment_api**
> `allocate_payment_api`(_api::`BookkeepingApi`, `allocate_payment_request`::`AllocatePaymentRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `allocate_payment_api`(_api::`BookkeepingApi`, response_stream::`Channel`, `allocate_payment_request`::`AllocatePaymentRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Allocate a payment to an invoice

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BookkeepingApi`** | API context | 
**`allocate_payment_request`** | [**`AllocatePaymentRequest`**](AllocatePaymentRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **bwa_report_api**
> `bwa_report_api`(_api::`BookkeepingApi`; `year`=nothing, `month`=nothing, _mediaType=nothing) -> `BWAReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `bwa_report_api`(_api::`BookkeepingApi`, response_stream::`Channel`; `year`=nothing, `month`=nothing, _mediaType=nothing) -> `Channel`{ `BWAReport` }, `OpenAPI.Clients.ApiResponse`

Get BWA (Betriebswirtschaftliche Auswertung) report

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BookkeepingApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`month`** | **`Int64`** |  | [default to nothing]

### Return type

[**`BWAReport`**](BWAReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **elster_status_api**
> `elster_status_api`(_api::`BookkeepingApi`; _mediaType=nothing) -> `ElsterStatus`, `OpenAPI.Clients.ApiResponse` <br/>
> `elster_status_api`(_api::`BookkeepingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `ElsterStatus` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`ElsterStatus`**](ElsterStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **elster_validate_api**
> `elster_validate_api`(_api::`BookkeepingApi`, `zeitraum`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `elster_validate_api`(_api::`BookkeepingApi`, response_stream::`Channel`, `zeitraum`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BookkeepingApi`** | API context | 
**`zeitraum`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **elster_xml_api**
> `elster_xml_api`(_api::`BookkeepingApi`, `zeitraum`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `elster_xml_api`(_api::`BookkeepingApi`, response_stream::`Channel`, `zeitraum`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BookkeepingApi`** | API context | 
**`zeitraum`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_cashflow**
> `get_cashflow`(_api::`BookkeepingApi`; `year`=nothing, `month`=nothing, _mediaType=nothing) -> `CashflowReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_cashflow`(_api::`BookkeepingApi`, response_stream::`Channel`; `year`=nothing, `month`=nothing, _mediaType=nothing) -> `Channel`{ `CashflowReport` }, `OpenAPI.Clients.ApiResponse`

GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BookkeepingApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`year`** | **`Int64`** |  | [default to nothing]
 **`month`** | **`Int64`** |  | [default to nothing]

### Return type

[**`CashflowReport`**](CashflowReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_liquidity**
> `get_liquidity`(_api::`BookkeepingApi`; _mediaType=nothing) -> `LiquidityPosition`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_liquidity`(_api::`BookkeepingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `LiquidityPosition` }, `OpenAPI.Clients.ApiResponse`

GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`LiquidityPosition`**](LiquidityPosition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_open_invoices_api**
> `get_open_invoices_api`(_api::`BookkeepingApi`, `customer_id`::`String`; _mediaType=nothing) -> `Vector{Invoice}`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_open_invoices_api`(_api::`BookkeepingApi`, response_stream::`Channel`, `customer_id`::`String`; _mediaType=nothing) -> `Channel`{ `Vector{Invoice}` }, `OpenAPI.Clients.ApiResponse`

Get open invoices for a customer

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BookkeepingApi`** | API context | 
**`customer_id`** | **`String`** |  |

### Return type

[**`Vector{Invoice}`**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **get_verfahrensdokumentation**
> `get_verfahrensdokumentation`(_api::`BookkeepingApi`; _mediaType=nothing) -> `Verfahrensdokumentation`, `OpenAPI.Clients.ApiResponse` <br/>
> `get_verfahrensdokumentation`(_api::`BookkeepingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Verfahrensdokumentation` }, `OpenAPI.Clients.ApiResponse`

GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`Verfahrensdokumentation`**](Verfahrensdokumentation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **run_dunning_api**
> `run_dunning_api`(_api::`BookkeepingApi`; _mediaType=nothing) -> `DunningResult`, `OpenAPI.Clients.ApiResponse` <br/>
> `run_dunning_api`(_api::`BookkeepingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `DunningResult` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`DunningResult`**](DunningResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

