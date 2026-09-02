# ServiceAssignment


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`employeeId`** | **`String`** | References the employees entity. | [optional] [default to nothing]
**`jobId`** | **`String`** | References the service_jobs entity. | [optional] [default to nothing]
**`notes`** | **`String`** |  | [optional] [default to nothing]
**`scheduledDate`** | **`Date`** | Work day the assignment is scheduled for. | [optional] [default to nothing]
**`scheduledEnd`** | **`String`** | Planned end time of the assignment. | [optional] [default to nothing]
**`scheduledStart`** | **`String`** | Planned start time of the assignment. | [optional] [default to nothing]
**`status`** | [**`*ServiceAssignmentStatus`**](ServiceAssignmentStatus.md) | Assignment lifecycle status: \&quot;planned\&quot;, \&quot;confirmed\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot; or \&quot;cancelled\&quot;. | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


