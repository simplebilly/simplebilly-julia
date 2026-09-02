# GenerateVariantsRequest


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`options`** | **`Dict{String, Vector{String}}`** | Option name → list of values, e.g. &#x60;{\&quot;Color\&quot;: [\&quot;Red\&quot;, \&quot;Blue\&quot;], \&quot;Size\&quot;: [\&quot;S\&quot;, \&quot;M\&quot;]}&#x60;. The cartesian product of these lists is generated. | [optional] [default to nothing]
**`priceDelta`** | **`String`** | Optional per-variant price delta applied to every generated variant. | [optional] [default to nothing]
**`productId`** | **`String`** |  | [default to nothing]
**`skuPrefix`** | **`String`** | Optional prefix for the generated SKUs (suffix is the option values joined by &#x60;-&#x60;). Falls back to the parent product&#39;s SKU. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


