# ReturnOrder


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`customerContactId`** | **`String`** | References the contact entity. | [optional] [default to nothing]
**`customerName`** | **`String`** |  | [optional] [default to nothing]
**`lineItems`** | **`Any`** | JSON array of &#x60;{product_id, name, quantity, condition, restock, batch_number?}&#x60;. | [optional] [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`orderId`** | **`String`** | References the order entity. | [optional] [default to nothing]
**`orderNumber`** | **`String`** |  | [optional] [default to nothing]
**`returnNumber`** | **`String`** |  | [default to nothing]
**`returnReason`** | **`String`** |  | [optional] [default to nothing]
**`status`** | [**`*ReturnOrderStatus`**](ReturnOrderStatus.md) | One of: requested | received | inspected | restocked | closed | [default to nothing]
**`warehouseId`** | **`String`** | Warehouse into which restockable items are returned. References the warehouse entity. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


