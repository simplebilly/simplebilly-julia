# Model


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`backup_codes`** | **`Vector{String}`** |  | [default to nothing]
**`created_at`** | **`ZonedDateTime`** |  | [default to nothing]
**`deleted_at`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`email`** | **`String`** |  | [default to nothing]
**`email_verified`** | **`Bool`** |  | [default to nothing]
**`id`** | **`String`** |  | [default to nothing]
**`is_active`** | **`Bool`** |  | [default to nothing]
**`is_totp_enabled`** | **`Bool`** |  | [default to nothing]
**`last_login`** | **`ZonedDateTime`** |  | [optional] [default to nothing]
**`name`** | **`String`** |  | [default to nothing]
**`oauth_id`** | **`String`** |  | [optional] [default to nothing]
**`oauth_provider`** | **`String`** |  | [optional] [default to nothing]
**`password_changed_at`** | **`ZonedDateTime`** | Set on password change; auth/refresh tokens issued before this timestamp are rejected by the auth middleware. | [optional] [default to nothing]
**`password_hash`** | **`String`** |  | [default to nothing]
**`picture`** | **`String`** |  | [optional] [default to nothing]
**`privacy_accepted_at`** | **`ZonedDateTime`** | When the user accepted the data privacy policy (GDPR consent record). | [optional] [default to nothing]
**`totp_secret`** | **`String`** |  | [optional] [default to nothing]
**`updated_at`** | **`ZonedDateTime`** |  | [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


