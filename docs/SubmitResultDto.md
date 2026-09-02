# SubmitResultDto


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`answers`** | **`Vector{Int64}`** | Selected answer indices (required for scored builtin trainings). | [default to nothing]
**`assignmentId`** | **`String`** |  | [optional] [default to nothing]
**`score`** | **`Int64`** | Score 0–100. Only trusted for plugin trainings without server-side scoring; builtin trainings are always re-scored from &#x60;answers&#x60;. | [default to nothing]
**`trainingCode`** | **`String`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


