# ProductVariantUpdate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`barcode`** | **`String`** |  | [optional] [default to nothing]
**`imageLink`** | **`String`** |  | [optional] [default to nothing]
**`isActive`** | **`Bool`** |  | [optional] [default to nothing]
**`name`** | **`String`** | Human-readable variant label, e.g. \&quot;Red / M\&quot;. | [optional] [default to nothing]
**`optionValues`** | **`Any`** | Option name → value map, e.g. &#x60;{\&quot;Color\&quot;: \&quot;Red\&quot;, \&quot;Size\&quot;: \&quot;M\&quot;}&#x60;. | [optional] [default to nothing]
**`price`** | **`String`** | Explicit override price for this variant (takes precedence over parent price + delta). | [optional] [default to nothing]
**`priceDelta`** | **`String`** | Price adjustment relative to the parent product&#39;s &#x60;default_price&#x60;. | [optional] [default to nothing]
**`productId`** | **`String`** | The parent product this variant belongs to. References the product entity. | [optional] [default to nothing]
**`sku`** | **`String`** | Variant-specific SKU (must be unique per tenant). | [optional] [default to nothing]
**`stockQuantity`** | **`Int64`** | Variant-level stock (optional — may be tracked on the parent only). | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


