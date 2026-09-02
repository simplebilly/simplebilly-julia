# ProformaInvoice


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`convertedAt`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`convertedToInvoiceId`** | **`String`** | Set when the proforma was converted into a real invoice. References the invoice entity. | [optional] [default to nothing]
**`currency`** | [**`*CurrencyCode`**](CurrencyCode.md) |  | [default to nothing]
**`customerId`** | **`String`** | References the customer entity. | [optional] [default to nothing]
**`customerSnapshot`** | **`Any`** | Snapshot of the recipient at issue time (address, VAT id, …). | [optional] [default to nothing]
**`issueDate`** | **`Date`** |  | [default to nothing]
**`lineItems`** | **`Any`** |  | [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`orderNumber`** | **`String`** | Reference to the order/quote this proforma belongs to. | [optional] [default to nothing]
**`paymentDueDate`** | **`Date`** | Optional deadline the real invoice should carry after conversion. | [optional] [default to nothing]
**`quotationId`** | **`String`** | References the quotation entity. | [optional] [default to nothing]
**`status`** | [**`*ProformaInvoiceStatus`**](ProformaInvoiceStatus.md) | &#x60;draft&#x60; | &#x60;sent&#x60; | &#x60;converted&#x60;. | [default to nothing]
**`subtotal`** | **`String`** |  | [default to nothing]
**`totalAmount`** | **`String`** |  | [default to nothing]
**`totalTax`** | **`String`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


