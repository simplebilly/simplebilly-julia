# StockTransfer


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`lineItems`** | **`Any`** | JSON array of &#x60;{product_id, name, quantity, batch_number?}&#x60;. | [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`sourceWarehouseId`** | **`String`** | References the warehouse entity. | [default to nothing]
**`status`** | [**`*StockTransferStatus`**](StockTransferStatus.md) | One of: draft | completed | cancelled | [default to nothing]
**`targetWarehouseId`** | **`String`** | References the warehouse entity. | [default to nothing]
**`transferDate`** | **`Date`** |  | [default to nothing]
**`transferNumber`** | **`String`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


