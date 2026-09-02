# StockMovement


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`delta`** | **`Int64`** | Signed movement: positive &#x3D; into stock, negative &#x3D; out of stock. | [default to nothing]
**`movementType`** | [**`*MovementType`**](MovementType.md) | One of the &#x60;MOVEMENT_*&#x60; constants. | [default to nothing]
**`productId`** | **`String`** | References the product entity. | [default to nothing]
**`quantity`** | **`Int64`** | Absolute quantity moved (always &gt;&#x3D; 0). | [default to nothing]
**`reason`** | **`String`** |  | [optional] [default to nothing]
**`referenceId`** | **`String`** | Primary-key of the referencing entity. | [optional] [default to nothing]
**`referenceType`** | [**`*ReferenceType`**](ReferenceType.md) | Entity that caused the movement, e.g. &#x60;goods_receipt&#x60;, &#x60;stock_transfer&#x60;. | [optional] [default to nothing]
**`warehouseId`** | **`String`** | References the warehouse entity. | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


