# WebhookEvent


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`attempts`** | **`Int64`** |  | [optional] [default to nothing]
**`channel`** | **`String`** | source for inbound, target URL for outbound. | [optional] [default to nothing]
**`direction`** | [**`*WebhookDirection`**](WebhookDirection.md) | inbound | outbound | [default to nothing]
**`eventType`** | **`String`** |  | [default to nothing]
**`lastError`** | **`String`** |  | [optional] [default to nothing]
**`payload`** | **`Any`** |  | [optional] [default to nothing]
**`status`** | [**`*WebhookEventStatus`**](WebhookEventStatus.md) | accepted | delivered | failed | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


