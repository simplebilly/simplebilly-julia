# BankingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bank_lookup_api**](BankingApi.md#bank_lookup_api) | **GET** /api/v1/bookkeeping/banking/lookup | 
[**bank_transactions_api**](BankingApi.md#bank_transactions_api) | **GET** /api/v1/bookkeeping/banking/transactions | 
[**hebesatz_lookup_api**](BankingApi.md#hebesatz_lookup_api) | **GET** /api/v1/bookkeeping/hebesatz | 


# **bank_lookup_api**
> `bank_lookup_api`(_api::`BankingApi`, `iban`::`String`; _mediaType=nothing) -> `BankLookup`, `OpenAPI.Clients.ApiResponse` <br/>
> `bank_lookup_api`(_api::`BankingApi`, response_stream::`Channel`, `iban`::`String`; _mediaType=nothing) -> `Channel`{ `BankLookup` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BankingApi`** | API context | 
**`iban`** | **`String`** |  |

### Return type

[**`BankLookup`**](BankLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **bank_transactions_api**
> `bank_transactions_api`(_api::`BankingApi`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `bank_transactions_api`(_api::`BankingApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters
This endpoint does not need any parameter.

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **hebesatz_lookup_api**
> `hebesatz_lookup_api`(_api::`BankingApi`; `gemeindeschluessel`=nothing, `plz`=nothing, `name`=nothing, `stichtag`=nothing, `country_code`=nothing, _mediaType=nothing) -> `Vector{HebesatzLookup}`, `OpenAPI.Clients.ApiResponse` <br/>
> `hebesatz_lookup_api`(_api::`BankingApi`, response_stream::`Channel`; `gemeindeschluessel`=nothing, `plz`=nothing, `name`=nothing, `stichtag`=nothing, `country_code`=nothing, _mediaType=nothing) -> `Channel`{ `Vector{HebesatzLookup}` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BankingApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`gemeindeschluessel`** | **`String`** |  | [default to nothing]
 **`plz`** | **`String`** |  | [default to nothing]
 **`name`** | **`String`** |  | [default to nothing]
 **`stichtag`** | **`String`** | Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from &lt;&#x3D; date &lt;&#x3D; valid_to. | [default to nothing]
 **`country_code`** | **`String`** |  | [default to nothing]

### Return type

[**`Vector{HebesatzLookup}`**](HebesatzLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

