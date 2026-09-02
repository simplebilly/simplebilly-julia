# TaxApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_tax_rate**](TaxApi.md#create_tax_rate) | **POST** /api/v1/tax-rates | Create a tax rate (&#x60;admin:settings&#x60;).
[**delete_tax_rate**](TaxApi.md#delete_tax_rate) | **DELETE** /api/v1/tax-rates/{id} | Delete a tax rate by id (&#x60;admin:settings&#x60;).
[**list_tax_rates**](TaxApi.md#list_tax_rates) | **GET** /api/v1/tax-rates | List the calling tenant&#39;s tax rates.
[**update_tax_rate**](TaxApi.md#update_tax_rate) | **PUT** /api/v1/tax-rates/{id} | Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields.


# **create_tax_rate**
> `create_tax_rate`(_api::`TaxApi`, `tax_rate_create`::`TaxRateCreate`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_tax_rate`(_api::`TaxApi`, response_stream::`Channel`, `tax_rate_create`::`TaxRateCreate`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Create a tax rate (`admin:settings`).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TaxApi`** | API context | 
**`tax_rate_create`** | [**`TaxRateCreate`**](TaxRateCreate.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **delete_tax_rate**
> `delete_tax_rate`(_api::`TaxApi`, `id`::`String`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `delete_tax_rate`(_api::`TaxApi`, response_stream::`Channel`, `id`::`String`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Delete a tax rate by id (`admin:settings`).

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TaxApi`** | API context | 
**`id`** | **`String`** |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **list_tax_rates**
> `list_tax_rates`(_api::`TaxApi`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `list_tax_rates`(_api::`TaxApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

List the calling tenant's tax rates.

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

# **update_tax_rate**
> `update_tax_rate`(_api::`TaxApi`, `id`::`String`, `tax_rate_create`::`TaxRateCreate`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `update_tax_rate`(_api::`TaxApi`, response_stream::`Channel`, `id`::`String`, `tax_rate_create`::`TaxRateCreate`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Update a tax rate by id (`admin:settings`). Replaces all body fields.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`TaxApi`** | API context | 
**`id`** | **`String`** |  |
**`tax_rate_create`** | [**`TaxRateCreate`**](TaxRateCreate.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

