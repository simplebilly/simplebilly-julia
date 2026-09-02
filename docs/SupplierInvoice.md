# SupplierInvoice


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`currency`** | **`String`** |  | [optional] [default to nothing]
**`goodsReceiptId`** | **`String`** | References the goods receipt entity. | [optional] [default to nothing]
**`invoiceDate`** | **`Date`** |  | [default to nothing]
**`invoiceNumber`** | **`String`** |  | [default to nothing]
**`lineItems`** | **`Any`** | JSON array of &#x60;{product_id, name, quantity, unitPriceNet, taxRate}&#x60;. | [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`purchaseOrderId`** | **`String`** | References the purchase order entity. | [optional] [default to nothing]
**`status`** | [**`*SupplierInvoiceStatus`**](SupplierInvoiceStatus.md) | One of: draft | matched | has_variances | posted | cancelled | [default to nothing]
**`supplierContactId`** | **`String`** | References the supplier entity. | [optional] [default to nothing]
**`supplierName`** | **`String`** |  | [optional] [default to nothing]
**`totalGrossAmount`** | **`String`** |  | [optional] [default to nothing]
**`totalNetAmount`** | **`String`** |  | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


