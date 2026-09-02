# Bom


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`components`** | **`Any`** | JSON array of &#x60;{product_id, name, quantity, unit, scrap_rate}&#x60;. | [optional] [default to nothing]
**`description`** | **`String`** |  | [optional] [default to nothing]
**`name`** | **`String`** |  | [default to nothing]
**`outputQuantity`** | **`Int64`** | Output quantity per production run (defaults to 1). | [optional] [default to nothing]
**`productId`** | **`String`** | The finished product this BOM produces. References the product entity. | [default to nothing]
**`status`** | [**`*BomStatus`**](BomStatus.md) | One of: draft | active | archived | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


