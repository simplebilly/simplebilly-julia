# JobPosting


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`currency`** | **`String`** |  | [optional] [default to nothing]
**`department`** | **`String`** |  | [optional] [default to nothing]
**`description`** | **`String`** | What the job is; markdown/HTML. | [default to nothing]
**`employmentType`** | [**`*EmploymentType`**](EmploymentType.md) | full_time | part_time | contract | internship | temporary | [optional] [default to nothing]
**`location`** | **`String`** |  | [optional] [default to nothing]
**`remote`** | **`Bool`** |  | [default to nothing]
**`requiredSkills`** | **`Any`** | List of required skill names (JSON array of strings). | [default to nothing]
**`requirements`** | **`String`** | Structured profile of the required candidate (skills, experience). | [optional] [default to nothing]
**`salaryMax`** | **`Int64`** |  | [optional] [default to nothing]
**`salaryMin`** | **`Int64`** |  | [optional] [default to nothing]
**`status`** | [**`*JobPostingStatus`**](JobPostingStatus.md) | draft | published | closed | [default to nothing]
**`title`** | **`String`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


