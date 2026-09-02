# ProductionOrderCosting


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`costPerUnit`** | **`String`** | material_cost_total ÷ quantity. | [default to nothing]
**`costSource`** | **`String`** | \&quot;actual\&quot; when costed from stock-movement consumption, else \&quot;planned\&quot;. | [default to nothing]
**`lines`** | [**`Vector{CostingLine}`**](CostingLine.md) |  | [default to nothing]
**`marginPerUnit`** | **`String`** | sale_price − cost_per_unit. | [optional] [default to nothing]
**`marginPercent`** | **`String`** | margin_per_unit ÷ cost_per_unit as a percentage. | [optional] [default to nothing]
**`materialCostTotal`** | **`String`** | Total material cost for the whole order. | [default to nothing]
**`orderNumber`** | **`String`** |  | [default to nothing]
**`productionOrderId`** | **`String`** |  | [default to nothing]
**`quantity`** | **`Int64`** |  | [default to nothing]
**`salePrice`** | **`String`** | Finished product&#39;s sale price per unit (used to compute margin). | [optional] [default to nothing]
**`status`** | **`String`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


