# EmissionEntry


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`activityValue`** | **`String`** | Activity amount in &#x60;unit&#x60; (kWh, l, km, t, tkm, EUR). | [default to nothing]
**`categoryId`** | **`String`** | GHG-Protocol category key, e.g. \&quot;purchased_goods\&quot;, \&quot;business_travel\&quot;. | [default to nothing]
**`description`** | **`String`** |  | [default to nothing]
**`efSource`** | **`String`** | Emission-factor source, e.g. \&quot;UBA-2024\&quot;, \&quot;DEFRA-2024\&quot;. | [default to nothing]
**`efVersion`** | **`String`** |  | [default to nothing]
**`method`** | [**`*EmissionMethod`**](EmissionMethod.md) | \&quot;activity\&quot; | \&quot;spend\&quot; | \&quot;supplier\&quot;. | [default to nothing]
**`scope`** | [**`*GhgScope`**](GhgScope.md) | GHG scope: \&quot;1\&quot; | \&quot;2\&quot; | \&quot;3\&quot;. | [default to nothing]
**`tco2e`** | **`String`** | Computed server-side: activity * factor / 1000, rounded to 4 dp. | [default to nothing]
**`unit`** | **`String`** | Unit of the activity value. | [default to nothing]
**`updatedAt`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`year`** | **`Int64`** | Reporting year. | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


