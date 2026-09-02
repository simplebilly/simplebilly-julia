# InventoryCountUpdate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`countDate`** | **`Date`** |  | [optional] [default to nothing]
**`countNumber`** | **`String`** |  | [optional] [default to nothing]
**`lineItems`** | **`Any`** | JSON array of &#x60;{product_id, name, sku, expected_quantity, counted_quantity, bin_location?, batch_number?, variance}&#x60;. | [optional] [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`status`** | [**`*InventoryCountStatus`**](InventoryCountStatus.md) | One of: draft | counting | reviewed | posted | [optional] [default to nothing]
**`warehouseId`** | **`String`** | References the warehouse entity. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


