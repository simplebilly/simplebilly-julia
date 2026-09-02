# SupplierConditionCreate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`currency`** | **`String`** | Currency for the minimum order value. | [default to nothing]
**`deliveryTerms`** | **`String`** | Incoterms, e.g. \&quot;EXW\&quot;, \&quot;DAP\&quot;. | [optional] [default to nothing]
**`earlyPaymentDiscountPercent`** | **`String`** | Early-payment discount percentage (Skonto), e.g. 2.0. | [optional] [default to nothing]
**`isDefault`** | **`Bool`** | Is this the default condition for the supplier? | [optional] [default to nothing]
**`minimumOrderValue`** | **`String`** | Minimum order value required for this supplier. | [optional] [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`paymentDueDays`** | **`Int64`** | Number of days within which payment is due. | [optional] [default to nothing]
**`paymentTerms`** | **`String`** | Payment terms, e.g. \&quot;14 Tage, 2% Skonto\&quot;. | [optional] [default to nothing]
**`supplierContactId`** | **`String`** | The supplier this condition applies to (&#x60;contact_id&#x60;). References the supplier entity. | [default to nothing]
**`supplierName`** | **`String`** | The name of the supplier, denormalized for easy listing. | [optional] [default to nothing]
**`volumeDiscountTiers`** | **`Any`** | Tiered discounts: JSON array of &#x60;{min_quantity, discount_percent}&#x60;. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


