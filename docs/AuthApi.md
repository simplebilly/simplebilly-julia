# AuthApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accept_invite**](AuthApi.md#accept_invite) | **POST** /auth/accept-invite | Accept an invite: create the account (or reuse an existing one) and join the inviting tenant. The invite token proves control of the mailbox.
[**forgot_password**](AuthApi.md#forgot_password) | **POST** /auth/forgot-password | Send a password reset email to the user
[**login**](AuthApi.md#login) | **POST** /auth/login | Authenticate a user with email + password (optional TOTP)
[**logout**](AuthApi.md#logout) | **POST** /auth/logout | Log out the current user (kills the assay session)
[**magic_link_login**](AuthApi.md#magic_link_login) | **POST** /auth/magic-link | Request a magic link login (sends an email with a one-time link)
[**magic_link_verify**](AuthApi.md#magic_link_verify) | **POST** /auth/magic-link/verify | Verify a magic link token and log the user in
[**register**](AuthApi.md#register) | **POST** /auth/register | Register a new user account
[**reset_password**](AuthApi.md#reset_password) | **POST** /auth/reset-password | Reset the user&#39;s password using a reset token
[**totp_enable**](AuthApi.md#totp_enable) | **POST** /auth/totp/enable | Enable TOTP two-factor authentication by verifying a code
[**totp_setup**](AuthApi.md#totp_setup) | **GET** /auth/totp/setup | Set up TOTP two-factor authentication (generates secret + backup codes)
[**verify_email**](AuthApi.md#verify_email) | **POST** /auth/verify-email | Verify a user&#39;s email address using a verification token


# **accept_invite**
> `accept_invite`(_api::`AuthApi`, `accept_invite_request`::`AcceptInviteRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `accept_invite`(_api::`AuthApi`, response_stream::`Channel`, `accept_invite_request`::`AcceptInviteRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Accept an invite: create the account (or reuse an existing one) and join the inviting tenant. The invite token proves control of the mailbox.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`accept_invite_request`** | [**`AcceptInviteRequest`**](AcceptInviteRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **forgot_password**
> `forgot_password`(_api::`AuthApi`, `forgot_password_request`::`ForgotPasswordRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `forgot_password`(_api::`AuthApi`, response_stream::`Channel`, `forgot_password_request`::`ForgotPasswordRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Send a password reset email to the user

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`forgot_password_request`** | [**`ForgotPasswordRequest`**](ForgotPasswordRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **login**
> `login`(_api::`AuthApi`, `login_request`::`LoginRequest`; _mediaType=nothing) -> `AuthResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `login`(_api::`AuthApi`, response_stream::`Channel`, `login_request`::`LoginRequest`; _mediaType=nothing) -> `Channel`{ `AuthResponse` }, `OpenAPI.Clients.ApiResponse`

Authenticate a user with email + password (optional TOTP)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`login_request`** | [**`LoginRequest`**](LoginRequest.md) |  |

### Return type

[**`AuthResponse`**](AuthResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **logout**
> `logout`(_api::`AuthApi`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `logout`(_api::`AuthApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Log out the current user (kills the assay session)

### Required Parameters
This endpoint does not need any parameter.

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **magic_link_login**
> `magic_link_login`(_api::`AuthApi`, `magic_link_request`::`MagicLinkRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `magic_link_login`(_api::`AuthApi`, response_stream::`Channel`, `magic_link_request`::`MagicLinkRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Request a magic link login (sends an email with a one-time link)

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`magic_link_request`** | [**`MagicLinkRequest`**](MagicLinkRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **magic_link_verify**
> `magic_link_verify`(_api::`AuthApi`, `magic_link_verify_request`::`MagicLinkVerifyRequest`; _mediaType=nothing) -> `AuthResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `magic_link_verify`(_api::`AuthApi`, response_stream::`Channel`, `magic_link_verify_request`::`MagicLinkVerifyRequest`; _mediaType=nothing) -> `Channel`{ `AuthResponse` }, `OpenAPI.Clients.ApiResponse`

Verify a magic link token and log the user in

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`magic_link_verify_request`** | [**`MagicLinkVerifyRequest`**](MagicLinkVerifyRequest.md) |  |

### Return type

[**`AuthResponse`**](AuthResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **register**
> `register`(_api::`AuthApi`, `register_request`::`RegisterRequest`; _mediaType=nothing) -> `AuthResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `register`(_api::`AuthApi`, response_stream::`Channel`, `register_request`::`RegisterRequest`; _mediaType=nothing) -> `Channel`{ `AuthResponse` }, `OpenAPI.Clients.ApiResponse`

Register a new user account

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`register_request`** | [**`RegisterRequest`**](RegisterRequest.md) |  |

### Return type

[**`AuthResponse`**](AuthResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **reset_password**
> `reset_password`(_api::`AuthApi`, `reset_password_request`::`ResetPasswordRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `reset_password`(_api::`AuthApi`, response_stream::`Channel`, `reset_password_request`::`ResetPasswordRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Reset the user's password using a reset token

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`reset_password_request`** | [**`ResetPasswordRequest`**](ResetPasswordRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **totp_enable**
> `totp_enable`(_api::`AuthApi`, `totp_enable_request`::`TotpEnableRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `totp_enable`(_api::`AuthApi`, response_stream::`Channel`, `totp_enable_request`::`TotpEnableRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Enable TOTP two-factor authentication by verifying a code

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`totp_enable_request`** | [**`TotpEnableRequest`**](TotpEnableRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **totp_setup**
> `totp_setup`(_api::`AuthApi`; _mediaType=nothing) -> `TotpSetupResponse`, `OpenAPI.Clients.ApiResponse` <br/>
> `totp_setup`(_api::`AuthApi`, response_stream::`Channel`; _mediaType=nothing) -> `Channel`{ `TotpSetupResponse` }, `OpenAPI.Clients.ApiResponse`

Set up TOTP two-factor authentication (generates secret + backup codes)

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**`TotpSetupResponse`**](TotpSetupResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

# **verify_email**
> `verify_email`(_api::`AuthApi`, `verify_email_request`::`VerifyEmailRequest`; _mediaType=nothing) -> `Nothing`, `OpenAPI.Clients.ApiResponse` <br/>
> `verify_email`(_api::`AuthApi`, response_stream::`Channel`, `verify_email_request`::`VerifyEmailRequest`; _mediaType=nothing) -> `Channel`{ `Nothing` }, `OpenAPI.Clients.ApiResponse`

Verify a user's email address using a verification token

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **_api** | **`AuthApi`** | API context | 
**`verify_email_request`** | [**`VerifyEmailRequest`**](VerifyEmailRequest.md) |  |

### Return type

`Nothing`

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

