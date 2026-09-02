# EmissionsReport


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`by_category`** | [**`Vector{CategoryTotal}`**](CategoryTotal.md) |  | [default to nothing]
**`by_scope`** | [**`Vector{ScopeTotal}`**](ScopeTotal.md) |  | [default to nothing]
**`by_year`** | [**`Vector{YearTotal}`**](YearTotal.md) |  | [default to nothing]
**`data_quality`** | [**`*DataQuality`**](DataQuality.md) |  | [default to nothing]
**`intensity_per_employee`** | **`Float64`** |  | [optional] [default to nothing]
**`intensity_per_revenue_mio`** | **`Float64`** | tCO2e per million EUR net revenue. | [optional] [default to nothing]
**`net_revenue`** | **`Float64`** | Sum of paid/sent/partially-paid invoices (EUR net) in the year. | [optional] [default to nothing]
**`spend_based_estimate_tco2e`** | **`Float64`** | Spend-based estimate from bookkeeping payments (EXIOBASE factor). | [optional] [default to nothing]
**`targets`** | [**`Vector{TargetProgress}`**](TargetProgress.md) |  | [default to nothing]
**`total_tco2e`** | **`String`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


