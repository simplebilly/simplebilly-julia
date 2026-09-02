# CreateSepaDirectDebitApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_sepa_direct_debit_api**](CreateSepaDirectDebitApi.md#create_sepa_direct_debit_api) | **POST** /api/v1/bookkeeping/sepa-direct-debit | 


# **create_sepa_direct_debit_api**
> `create_sepa_direct_debit_api`(_api::`CreateSepaDirectDebitApi`, `creditor_name`::`String`, `creditor_iban`::`String`, `creditor_id`::`String`, `mandate_id`::`String`, `mandate_date`::`String`, `debtor_name`::`String`, `debtor_iban`::`String`, `amount`::`String`, `collection_date`::`String`; `creditor_bic`=nothing, `debtor_bic`=nothing, `description`=nothing, _mediaType=nothing) -> `SepaDirectDebitResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `create_sepa_direct_debit_api`(_api::`CreateSepaDirectDebitApi`, response_stream::`Channel`, `creditor_name`::`String`, `creditor_iban`::`String`, `creditor_id`::`String`, `mandate_id`::`String`, `mandate_date`::`String`, `debtor_name`::`String`, `debtor_iban`::`String`, `amount`::`String`, `collection_date`::`String`; `creditor_bic`=nothing, `debtor_bic`=nothing, `description`=nothing, _mediaType=nothing) -> `Channel`{ `SepaDirectDebitResponse` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`CreateSepaDirectDebitApi`** | API context | 
**`creditor_name`** | **`String`** |  |
**`creditor_iban`** | **`String`** |  |
**`creditor_id`** | **`String`** |  |
**`mandate_id`** | **`String`** |  |
**`mandate_date`** | **`String`** |  |
**`debtor_name`** | **`String`** |  |
**`debtor_iban`** | **`String`** |  |
**`amount`** | **`String`** |  |
**`collection_date`** | **`String`** |  |

### Optional Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **`creditor_bic`** | **`String`** |  | [default to nothing]
 **`debtor_bic`** | **`String`** |  | [default to nothing]
 **`description`** | **`String`** |  | [default to nothing]

### Return type

[**`SepaDirectDebitResponse`**](SepaDirectDebitResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

