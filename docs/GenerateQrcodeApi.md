# GenerateQrcodeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_qrcode_api**](GenerateQrcodeApi.md#generate_qrcode_api) | **GET** /api/v1/invoices/{id}/qrcode | 


# **generate_qrcode_api**
> `generate_qrcode_api`(_api::`GenerateQrcodeApi`, `iban`::`String`, `id`::`String`; `holder_name`=nothing, `bic`=nothing, `amount`=nothing, `reference`=nothing, `purpose`=nothing, _mediaType=nothing) -> `QRCodeResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `generate_qrcode_api`(_api::`GenerateQrcodeApi`, response_stream::`Channel`, `iban`::`String`, `id`::`String`; `holder_name`=nothing, `bic`=nothing, `amount`=nothing, `reference`=nothing, `purpose`=nothing, _mediaType=nothing) -> `Channel`{ `QRCodeResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GenerateQrcodeApi`** | API context | 
**`iban`** | **`String`** |  |
**`id`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`holder_name`** | **`String`** |  | [default to nothing]
 **`bic`** | **`String`** |  | [default to nothing]
 **`amount`** | **`String`** |  | [default to nothing]
 **`reference`** | **`String`** |  | [default to nothing]
 **`purpose`** | **`String`** |  | [default to nothing]

### Return type

[**`QRCodeResponse`**](QRCodeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

