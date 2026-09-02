# JobApplication


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`cvFile`** | **`String`** | Relative path of the stored CV file under the upload dir. | [optional] [default to nothing]
**`cvText`** | **`String`** | Extracted CV text, used for match-scoring. | [optional] [default to nothing]
**`email`** | **`String`** |  | [optional] [default to nothing]
**`matchReason`** | **`String`** |  | [optional] [default to nothing]
**`matchScore`** | **`Int64`** | 0-100 LLM match score against the posting&#39;s required profile. | [optional] [default to nothing]
**`name`** | **`String`** |  | [optional] [default to nothing]
**`phone`** | **`String`** |  | [optional] [default to nothing]
**`postingId`** | **`String`** | References the job_posting entity. | [optional] [default to nothing]
**`source`** | **`String`** | website | email | board | [default to nothing]
**`status`** | [**`*ApplicationStatus`**](ApplicationStatus.md) | new | reviewing | interview | hired | rejected | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


