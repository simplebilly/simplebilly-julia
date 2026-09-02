# ImportJobStatus


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`error`** | **`String`** | Set only when the job failed. | [optional] [default to nothing]
**`job_id`** | **`String`** |  | [default to nothing]
**`processed`** | **`Int64`** |  | [default to nothing]
**`progress`** | **`Int64`** | 0–100 | [default to nothing]
**`provider`** | **`String`** | Which competitor the import came from (lexoffice | billbee); the frontend uses it to label the job. Absent for legacy jobs. | [optional] [default to nothing]
**`stage`** | **`String`** | queued | fetching | downloading | importing | done | [default to nothing]
**`status`** | **`String`** | pending | running | done | failed | [default to nothing]
**`total`** | **`Int64`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


