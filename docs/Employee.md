# Employee


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`address`** | **`String`** |  | [optional] [default to nothing]
**`backupEmployeeId`** | **`String`** | References another employee who covers when this employee is absent. | [optional] [default to nothing]
**`bic`** | **`String`** |  | [optional] [default to nothing]
**`city`** | **`String`** |  | [optional] [default to nothing]
**`country`** | [**`*CountryCode`**](CountryCode.md) |  | [optional] [default to nothing]
**`createdAt`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`dateOfBirth`** | **`Date`** |  | [optional] [default to nothing]
**`deletedAt`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`departmentId`** | **`String`** | References the department entity. | [optional] [default to nothing]
**`email`** | **`String`** |  | [optional] [default to nothing]
**`firstName`** | **`String`** |  | [optional] [default to nothing]
**`gender`** | [**`*Gender`**](Gender.md) | Gender for pay-transparency reporting: \&quot;male\&quot;, \&quot;female\&quot; or \&quot;diverse\&quot;. | [optional] [default to nothing]
**`hireDate`** | **`Date`** |  | [optional] [default to nothing]
**`hourlyCost`** | **`String`** | Hourly cost rate in EUR for labor-cost reporting; when unset the rate is derived from &#x60;monthly_salary / (weekly_hours * 4.33)&#x60;. | [optional] [default to nothing]
**`iban`** | **`String`** |  | [optional] [default to nothing]
**`id`** | **`String`** |  | [optional] [default to nothing]
**`jobTitle`** | **`String`** |  | [optional] [default to nothing]
**`lastLogin`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`lastName`** | **`String`** |  | [optional] [default to nothing]
**`lastUpdated`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`monthlySalary`** | **`String`** | Gross monthly salary in EUR for pay-transparency reporting. | [optional] [default to nothing]
**`phone`** | **`String`** |  | [optional] [default to nothing]
**`state`** | **`String`** |  | [optional] [default to nothing]
**`status`** | [**`*EmployeeStatus`**](EmployeeStatus.md) |  | [optional] [default to nothing]
**`tenantId`** | **`String`** |  | [optional] [default to nothing]
**`updatedAt`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`userId`** | **`String`** | References the user entity. | [optional] [default to nothing]
**`weeklyHours`** | **`String`** | Contractual weekly working hours for pay-transparency normalization. | [optional] [default to nothing]
**`zip`** | **`String`** |  | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


