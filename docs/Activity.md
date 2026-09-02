# Activity


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`activityType`** | [**`*ActivityType`**](ActivityType.md) | One of: call | email | meeting | task | note | [default to nothing]
**`assignedTo`** | **`String`** | User responsible (&#x60;employee.employee_id&#x60;). | [optional] [default to nothing]
**`contactId`** | **`String`** | Contact this activity belongs to (&#x60;contact.contact_id&#x60;). References the contact entity. | [optional] [default to nothing]
**`description`** | **`String`** |  | [optional] [default to nothing]
**`dueDate`** | **`Date`** | Follow-up / Wiedervorlage date. Open activities with a due date in the past are overdue. | [optional] [default to nothing]
**`reminderDate`** | **`Date`** | When to remind about the follow-up. | [optional] [default to nothing]
**`status`** | [**`*ActivityStatus`**](ActivityStatus.md) | One of: open | done | cancelled | [default to nothing]
**`subject`** | **`String`** | Short subject line. | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


