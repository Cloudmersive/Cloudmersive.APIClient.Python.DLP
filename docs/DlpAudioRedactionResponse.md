# DlpAudioRedactionResponse

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**redacted_audio** | **str** | The redacted audio file bytes with PII segments bleeped or muted, or the original audio if no disallowed PII was found. | [optional] 
**redacted_transcript** | **str** | The redacted transcript text with PII removed or replaced. | [optional] 
**original_transcript** | **str** | Full original transcript of the audio file. | [optional] 
**timestamps** | [**list[AudioTimestamp]**](AudioTimestamp.md) | Token-level timestamps from speech recognition. | [optional] 
**redacted_segments** | [**list[RedactedAudioSegment]**](RedactedAudioSegment.md) | List of audio segments that were redacted, with their time ranges. | [optional] 
**clean_result** | **bool** | True if no disallowed PII or sensitive data types were detected; false if any disallowed type was found and redacted. | [optional] 
**contains_email_address** | **bool** | True if the audio transcript contains email addresses. | [optional] 
**contains_phone_number** | **bool** | True if the audio transcript contains phone numbers. | [optional] 
**contains_street_address** | **bool** | True if the audio transcript contains street addresses. | [optional] 
**contains_person_name** | **bool** | True if the audio transcript contains person names. | [optional] 
**contains_birth_date** | **bool** | True if the audio transcript contains birth dates. | [optional] 
**contains_passport_number** | **bool** | True if the audio transcript contains passport numbers. | [optional] 
**contains_drivers_license** | **bool** | True if the audio transcript contains drivers license numbers. | [optional] 
**contains_social_security_number** | **bool** | True if the audio transcript contains social security numbers. | [optional] 
**contains_taxpayer_id** | **bool** | True if the audio transcript contains taxpayer IDs. | [optional] 
**contains_credit_card_number** | **bool** | True if the audio transcript contains credit card numbers. | [optional] 
**contains_credit_card_expiration_date** | **bool** | True if the audio transcript contains credit card expiration dates. | [optional] 
**contains_credit_card_verification_code** | **bool** | True if the audio transcript contains credit card verification codes. | [optional] 
**contains_bank_account_number** | **bool** | True if the audio transcript contains bank account numbers. | [optional] 
**contains_iban** | **bool** | True if the audio transcript contains IBANs. | [optional] 
**contains_health_insurance_number** | **bool** | True if the audio transcript contains health insurance numbers. | [optional] 
**contains_bearer_token** | **bool** | True if the audio transcript contains bearer tokens. | [optional] 
**contains_http_cookie** | **bool** | True if the audio transcript contains HTTP cookies. | [optional] 
**contains_private_keys** | **bool** | True if the audio transcript contains private keys. | [optional] 
**contains_credentials** | **bool** | True if the audio transcript contains credentials (usernames/passwords). | [optional] 
**contains_deep_web_urls** | **bool** | True if the audio transcript contains deep web URLs (.onion). | [optional] 
**contains_source_code** | **bool** | True if the audio transcript contains source code. | [optional] 
**contains_ip_address** | **bool** | True if the audio transcript contains IP addresses. | [optional] 
**contains_mac_address** | **bool** | True if the audio transcript contains MAC addresses. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


