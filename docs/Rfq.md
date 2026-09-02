# Rfq


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`currency`** | **`String`** |  | [optional] [default to nothing]
**`lineItems`** | **`Any`** | JSON array of &#x60;{product_id, name, sku, quantity, requested_unit_price?, quoted_unit_price?}&#x60;. | [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`requestedDate`** | **`Date`** |  | [default to nothing]
**`responseDate`** | **`Date`** |  | [optional] [default to nothing]
**`rfqNumber`** | **`String`** |  | [default to nothing]
**`status`** | [**`*RfqStatus`**](RfqStatus.md) | One of: draft | sent | offer_received | rejected | converted | [default to nothing]
**`supplierContactId`** | **`String`** | References the supplier entity. | [optional] [default to nothing]
**`supplierName`** | **`String`** |  | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


