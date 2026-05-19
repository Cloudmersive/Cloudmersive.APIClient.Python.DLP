# DlpAudioRedactionRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input_file** | **str** | Audio file bytes (WAV, MP3, M4A, FLAC, OGG, or WMA) to transcribe, scan for PII, and redact. | [optional] 
**language_code** | **str** | Language code for speech recognition. Default is \&quot;ENG\&quot; (English). | [optional] 
**allow_email_address** | **bool** | Set to true to allow email addresses in the audio transcript and not redact them. | [optional] 
**allow_phone_number** | **bool** | Set to true to allow phone numbers in the audio transcript and not redact them. | [optional] 
**allow_street_address** | **bool** | Set to true to allow street addresses in the audio transcript and not redact them. | [optional] 
**allow_person_name** | **bool** | Set to true to allow person names in the audio transcript and not redact them. | [optional] 
**allow_birth_date** | **bool** | Set to true to allow birth dates in the audio transcript and not redact them. | [optional] 
**allow_passport_number** | **bool** | Set to true to allow passport numbers in the audio transcript and not redact them. | [optional] 
**allow_drivers_license** | **bool** | Set to true to allow drivers license numbers in the audio transcript and not redact them. | [optional] 
**allow_social_security_number** | **bool** | Set to true to allow social security numbers in the audio transcript and not redact them. | [optional] 
**allow_taxpayer_id** | **bool** | Set to true to allow taxpayer IDs in the audio transcript and not redact them. | [optional] 
**allow_credit_card_number** | **bool** | Set to true to allow credit card numbers in the audio transcript and not redact them. | [optional] 
**allow_credit_card_expiration_date** | **bool** | Set to true to allow credit card expiration dates in the audio transcript and not redact them. | [optional] 
**allow_credit_card_verification_code** | **bool** | Set to true to allow credit card verification codes in the audio transcript and not redact them. | [optional] 
**allow_bank_account_number** | **bool** | Set to true to allow bank account numbers in the audio transcript and not redact them. | [optional] 
**allow_iban** | **bool** | Set to true to allow IBANs in the audio transcript and not redact them. | [optional] 
**allow_health_insurance_number** | **bool** | Set to true to allow health insurance numbers in the audio transcript and not redact them. | [optional] 
**allow_bearer_token** | **bool** | Set to true to allow bearer tokens in the audio transcript and not redact them. | [optional] 
**allow_http_cookie** | **bool** | Set to true to allow HTTP cookies in the audio transcript and not redact them. | [optional] 
**allow_private_keys** | **bool** | Set to true to allow private keys in the audio transcript and not redact them. | [optional] 
**allow_credentials** | **bool** | Set to true to allow credentials (usernames/passwords) in the audio transcript and not redact them. | [optional] 
**allow_deep_web_urls** | **bool** | Set to true to allow deep web URLs (.onion) in the audio transcript and not redact them. | [optional] 
**allow_source_code** | **bool** | Set to true to allow source code in the audio transcript and not redact it. | [optional] 
**allow_ip_address** | **bool** | Set to true to allow IP addresses in the audio transcript and not redact them. | [optional] 
**allow_mac_address** | **bool** | Set to true to allow MAC addresses in the audio transcript and not redact them. | [optional] 
**redaction_mode** | **str** | Redaction mode for audio: \&quot;Bleep\&quot; (default) replaces redacted audio segments with a bleep tone, or \&quot;Mute\&quot; zeroes out the audio for the redacted portions. | [optional] 
**transcript_redaction_mode** | **str** | Redaction mode for the transcript text: \&quot;SemanticTag\&quot; (default) replaces PII with a semantic tag in square brackets (e.g. [PHONE-NUMBER]), \&quot;Delete\&quot; removes PII entirely, or \&quot;ReplaceWithAsterisk\&quot; replaces PII characters with asterisks (*). | [optional] 
**speech_recognition_mode** | **str** | Optional. Speech recognition mode used when transcribing the audio for redaction. Available values: \&quot;Fast\&quot;, \&quot;Normal\&quot;, or \&quot;Advanced\&quot;. Defaults to \&quot;Normal\&quot; when not specified. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


