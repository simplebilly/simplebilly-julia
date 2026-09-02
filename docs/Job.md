# Job


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`attempts`** | **`Int64`** |  | [optional] [default to nothing]
**`jobType`** | **`String`** | Discriminator the worker dispatches on (e.g. \&quot;webhook.deliver\&quot;). | [default to nothing]
**`maxAttempts`** | **`Int64`** |  | [default to nothing]
**`payload`** | **`Any`** |  | [optional] [default to nothing]
**`runAt`** | **`ZonedDateTime`** | Earliest execution time; None &#x3D; run now. | [optional] [default to nothing]
**`status`** | [**`*JobStatus`**](JobStatus.md) | pending | running | done | failed | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


