# TaxRateCreate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`countryCode`** | **`String`** | ISO 3166-1 alpha-2 country code. | [default to nothing]
**`effectiveFrom`** | **`Date`** | Date this rate took effect; &#x60;None&#x60; &#x3D; not date-bound. | [optional] [default to nothing]
**`isDefault`** | **`Bool`** | Default rate for the country (one per country); fallback for lookups when no dated rate applies. | [default to nothing]
**`name`** | **`String`** | Human name, e.g. \&quot;VAT\&quot;. | [default to nothing]
**`ratePercent`** | **`Int64`** | Rate in hundredths of a percent: 1900 &#x3D; 19.00%. | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


