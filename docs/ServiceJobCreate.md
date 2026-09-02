# ServiceJobCreate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`address`** | **`String`** | Street + zip + city of the job location. | [optional] [default to nothing]
**`customerEmail`** | **`String`** | Customer email for email notifications. | [optional] [default to nothing]
**`customerId`** | **`String`** | References the customer entity. | [optional] [default to nothing]
**`customerName`** | **`String`** | Denormalized customer name for quick display. | [optional] [default to nothing]
**`customerPhone`** | **`String`** | Customer phone for SMS notifications later. | [optional] [default to nothing]
**`description`** | **`String`** | What work needs to be done. | [optional] [default to nothing]
**`estimatedDurationMinutes`** | **`Int64`** | Estimated time for the job in minutes. | [optional] [default to nothing]
**`lat`** | **`Float64`** | Latitude for map display (OpenStreetMap). | [optional] [default to nothing]
**`lng`** | **`Float64`** | Longitude for map display (OpenStreetMap). | [optional] [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`status`** | [**`*ServiceJobStatus`**](ServiceJobStatus.md) | Dispatch status: \&quot;pending\&quot;, \&quot;assigned\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot;, \&quot;cancelled\&quot;. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


