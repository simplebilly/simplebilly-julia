# PurchaseOrderCreate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`currency`** | **`String`** |  | [optional] [default to nothing]
**`deliveryAddress`** | **`Any`** |  | [optional] [default to nothing]
**`expectedDeliveryDate`** | **`Date`** |  | [optional] [default to nothing]
**`lineItems`** | **`Any`** | JSON array of &#x60;{product_id, name, quantity, unit_price_net, tax_rate, delivery_date}&#x60;. | [optional] [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`orderDate`** | **`Date`** |  | [default to nothing]
**`poNumber`** | **`String`** |  | [default to nothing]
**`status`** | [**`*PurchaseOrderStatus`**](PurchaseOrderStatus.md) | One of: draft | ordered | partially_received | received | cancelled | [default to nothing]
**`supplierContactId`** | **`String`** | References the supplier entity. | [optional] [default to nothing]
**`supplierName`** | **`String`** |  | [optional] [default to nothing]
**`totalGrossAmount`** | **`String`** |  | [optional] [default to nothing]
**`totalNetAmount`** | **`String`** |  | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


