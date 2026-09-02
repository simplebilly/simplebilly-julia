# ProductionOrder


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`bomId`** | **`String`** | References the BOM entity. | [optional] [default to nothing]
**`components`** | **`Any`** | JSON snapshot of the BOM components at creation time. | [optional] [default to nothing]
**`endDate`** | **`Date`** |  | [optional] [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`orderNumber`** | **`String`** |  | [default to nothing]
**`productId`** | **`String`** | The finished product to manufacture. References the product entity. | [default to nothing]
**`quantity`** | **`Int64`** | Quantity of finished product to produce. | [default to nothing]
**`sourceWarehouseId`** | **`String`** | Warehouse components are consumed from. References the warehouse entity. | [optional] [default to nothing]
**`startDate`** | **`Date`** |  | [optional] [default to nothing]
**`status`** | [**`*ProductionOrderStatus`**](ProductionOrderStatus.md) | One of: planned | in_production | completed | cancelled | [optional] [default to nothing]
**`targetWarehouseId`** | **`String`** | Warehouse the finished product is added to. References the warehouse entity. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


