# GezApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gez_api**](GezApi.md#gez_api) | **GET** /api/v1/bookkeeping/gez | 


# **gez_api**
> `gez_api`(_api::`GezApi`; `jahr`=nothing, `betriebsstaetten`=nothing, `kfz`=nothing, `hotelzimmer`=nothing, `beschaefigte`=nothing, _mediaType=nothing) -> `GezReport`, `OpenAPI.Clients.ApiResponse` <br/>
> `gez_api`(_api::`GezApi`, response_stream::`Channel`; `jahr`=nothing, `betriebsstaetten`=nothing, `kfz`=nothing, `hotelzimmer`=nothing, `beschaefigte`=nothing, _mediaType=nothing) -> `Channel`{ `GezReport` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`GezApi`** | API context | 

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`jahr`** | **`Int64`** |  | [default to nothing]
 **`betriebsstaetten`** | **`String`** | Liste der Betriebsstätten als JSON, z.B. &#x60;[{\&quot;name\&quot;:\&quot;Filiale 1\&quot;,\&quot;beschaefigte\&quot;:12}]&#x60;. | [default to nothing]
 **`kfz`** | **`Int64`** | Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). | [default to nothing]
 **`hotelzimmer`** | **`Int64`** | Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. | [default to nothing]
 **`beschaefigte`** | **`Int64`** | Gesamtzahl der Beschäftigten (verwendet nur, wenn &#x60;betriebsstaetten&#x60; fehlt; dann wird eine einzelne Betriebsstätte angenommen). | [default to nothing]

### Return type

[**`GezReport`**](GezReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

