# InventoryCountCreate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`countDate`** | **`Date`** |  | [default to nothing]
**`countNumber`** | **`String`** |  | [default to nothing]
**`lineItems`** | **`Any`** | JSON array of &#x60;{product_id, name, sku, expected_quantity, counted_quantity, bin_location?, batch_number?, variance}&#x60;. | [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`status`** | [**`*InventoryCountStatus`**](InventoryCountStatus.md) | One of: draft | counting | reviewed | posted | [default to nothing]
**`warehouseId`** | **`String`** | References the warehouse entity. | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


