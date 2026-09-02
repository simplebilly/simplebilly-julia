# CustomerCommunicationCreate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`body`** | **`String`** | The message body, call summary or note text. | [optional] [default to nothing]
**`channel`** | [**`*CommunicationChannel`**](CommunicationChannel.md) |  | [default to nothing]
**`contactId`** | **`String`** | The contact (customer/supplier) this communication belongs to. References the contact entity. | [default to nothing]
**`counterparty`** | **`String`** | Email/phone of the counterparty, if applicable. | [optional] [default to nothing]
**`direction`** | [**`*CommunicationDirection`**](CommunicationDirection.md) |  | [default to nothing]
**`occurredAt`** | **`ZonedDateTime`** | When the communication happened (defaults to now on create). | [optional] [default to nothing]
**`subject`** | **`String`** |  | [optional] [default to nothing]
**`tags`** | **`Any`** | Free-form tags, e.g. &#x60;[\&quot;follow-up-required\&quot;]&#x60;. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


