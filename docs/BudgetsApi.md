# BudgetsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**budgets_api**](BudgetsApi.md#budgets_api) | **GET** /api/v1/bookkeeping/budgets | 
[**upsert_budget_goal_api**](BudgetsApi.md#upsert_budget_goal_api) | **PUT** /api/v1/bookkeeping/budgets/goals/{category} | 


# **budgets_api**
> `budgets_api`(_api::`BudgetsApi`, `year`::`Int64`, `month`::`Int64`; _mediaType=nothing) -> `BudgetErgebnis`, `OpenAPI.Clients.ApiResponse` <br/>
> `budgets_api`(_api::`BudgetsApi`, response_stream::`Channel`, `year`::`Int64`, `month`::`Int64`; _mediaType=nothing) -> `Channel`{ `BudgetErgebnis` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BudgetsApi`** | API context | 
**`year`** | **`Int64`** |  |
**`month`** | **`Int64`** |  |

### Return type

[**`BudgetErgebnis`**](BudgetErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **upsert_budget_goal_api**
> `upsert_budget_goal_api`(_api::`BudgetsApi`, `category`::`String`, `budget_goal_request`::`BudgetGoalRequest`; _mediaType=nothing) -> `Budget`, `OpenAPI.Clients.ApiResponse` <br/>
> `upsert_budget_goal_api`(_api::`BudgetsApi`, response_stream::`Channel`, `category`::`String`, `budget_goal_request`::`BudgetGoalRequest`; _mediaType=nothing) -> `Channel`{ `Budget` }, `OpenAPI.Clients.ApiResponse`



### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`BudgetsApi`** | API context | 
**`category`** | **`String`** |  |
**`budget_goal_request`** | [**`BudgetGoalRequest`**](BudgetGoalRequest.md) |  |

### Return type

[**`Budget`**](Budget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

