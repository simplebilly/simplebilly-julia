# ShippingRuleCreate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`carrier`** | **`String`** | Provider that auto-filled this rule (e.g. \&quot;ups\&quot;), if any. | [optional] [default to nothing]
**`country`** | [**`*CountryCode`**](CountryCode.md) | None &#x3D; applies to all countries. | [optional] [default to nothing]
**`deliveryTime`** | **`String`** | Delivery time text, e.g. \&quot;1-3\&quot;. | [optional] [default to nothing]
**`isActive`** | **`Bool`** |  | [optional] [default to nothing]
**`maxWeightKg`** | **`Float64`** |  | [optional] [default to nothing]
**`minWeightKg`** | **`Float64`** |  | [optional] [default to nothing]
**`name`** | **`String`** | Delivery-method label, e.g. \&quot;Standardversand\&quot;. | [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`price`** | **`String`** | Shipping cost in the shop&#39;s currency. | [default to nothing]
**`priority`** | **`Int64`** | Lower wins when multiple rules match. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


