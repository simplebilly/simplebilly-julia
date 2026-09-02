# PluginPricing



## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | This is a oneOf model. The value must be exactly one of the following types: PluginPricingOneOf, PluginPricingOneOf1, PluginPricingOneOf2 | How a plugin is priced in the marketplace. Tagged on &#x60;type&#x60; so the same enum deserializes both the API DTO and the &#x60;plugin_marketplace.json&#x60; manifest (&#x60;{\&quot;type\&quot;:\&quot;free\&quot;}&#x60; / &#x60;{\&quot;type\&quot;:\&quot;one_time\&quot;,\&quot;price\&quot;:99.0}&#x60; / &#x60;{\&quot;type\&quot;:\&quot;recurring\&quot;,\&quot;price_per_month\&quot;:19.9}&#x60;). | [optional] 




[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


