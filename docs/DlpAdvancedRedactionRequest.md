# DlpAdvancedRedactionRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input_text** | **str** | Text to scan for PII and redact sensitive data from. | [optional] 
**allow_email_address** | **bool** | Set to true to allow email addresses in the input text and not redact them. | [optional] 
**allow_phone_number** | **bool** | Set to true to allow phone numbers in the input text and not redact them. | [optional] 
**allow_street_address** | **bool** | Set to true to allow street addresses in the input text and not redact them. | [optional] 
**allow_person_name** | **bool** | Set to true to allow person names in the input text and not redact them. | [optional] 
**allow_birth_date** | **bool** | Set to true to allow birth dates in the input text and not redact them. | [optional] 
**allow_passport_number** | **bool** | Set to true to allow passport numbers in the input text and not redact them. | [optional] 
**allow_drivers_license** | **bool** | Set to true to allow drivers license numbers in the input text and not redact them. | [optional] 
**allow_social_security_number** | **bool** | Set to true to allow social security numbers in the input text and not redact them. | [optional] 
**allow_taxpayer_id** | **bool** | Set to true to allow taxpayer IDs in the input text and not redact them. | [optional] 
**allow_credit_card_number** | **bool** | Set to true to allow credit card numbers in the input text and not redact them. | [optional] 
**allow_credit_card_expiration_date** | **bool** | Set to true to allow credit card expiration dates in the input text and not redact them. | [optional] 
**allow_credit_card_verification_code** | **bool** | Set to true to allow credit card verification codes in the input text and not redact them. | [optional] 
**allow_bank_account_number** | **bool** | Set to true to allow bank account numbers in the input text and not redact them. | [optional] 
**allow_iban** | **bool** | Set to true to allow IBANs in the input text and not redact them. | [optional] 
**allow_health_insurance_number** | **bool** | Set to true to allow health insurance numbers in the input text and not redact them. | [optional] 
**allow_bearer_token** | **bool** | Set to true to allow bearer tokens in the input text and not redact them. | [optional] 
**allow_http_cookie** | **bool** | Set to true to allow HTTP cookies in the input text and not redact them. | [optional] 
**allow_private_keys** | **bool** | Set to true to allow private keys in the input text and not redact them. | [optional] 
**allow_credentials** | **bool** | Set to true to allow credentials (usernames/passwords) in the input text and not redact them. | [optional] 
**allow_deep_web_urls** | **bool** | Set to true to allow deep web URLs (.onion) in the input text and not redact them. | [optional] 
**allow_source_code** | **bool** | Set to true to allow source code in the input text and not redact it. | [optional] 
**allow_ip_address** | **bool** | Set to true to allow IP addresses in the input text and not redact them. | [optional] 
**allow_mac_address** | **bool** | Set to true to allow MAC addresses in the input text and not redact them. | [optional] 
**allow_health_insurance_member_id** | **bool** | Set to true to allow health insurance member IDs in the input text and not redact them. | [optional] 
**allow_health_injury_or_disease** | **bool** | Set to true to allow references to injuries or diseases in the input text and not redact them. | [optional] 
**allow_health_type_of_treatment** | **bool** | Set to true to allow references to types of medical treatment in the input text and not redact them. | [optional] 
**allow_health_date_and_time_of_treatment** | **bool** | Set to true to allow dates and times of medical treatment in the input text and not redact them. | [optional] 
**allow_health_plan_beneficiary_number** | **bool** | Set to true to allow health plan beneficiary numbers in the input text and not redact them. | [optional] 
**allow_health_payments_made_for_treatment** | **bool** | Set to true to allow payments made for medical treatment in the input text and not redact them. | [optional] 
**allow_vehicle_id** | **bool** | Set to true to allow vehicle identifiers (e.g. license plates, VINs) in the input text and not redact them. | [optional] 
**allow_device_id** | **bool** | Set to true to allow device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs) in the input text and not redact them. | [optional] 
**allow_names_of_relatives** | **bool** | Set to true to allow names of relatives in the input text and not redact them. | [optional] 
**allow_health_universal_record_locator** | **bool** | Set to true to allow health universal record locators (URLs) in the input text and not redact them. | [optional] 
**allow_biometrics** | **bool** | Set to true to allow biometric data references (e.g. fingerprints, retinal scans, voiceprints) in the input text and not redact them. | [optional] 
**redaction_mode** | **str** | Redaction mode: \&quot;Delete\&quot; to remove PII entirely, or \&quot;ReplaceWithAsterisk\&quot; to replace PII characters with asterisks (*). | [optional] 
**provide_analysis_rationale** | **bool** | Set to true to include a natural language rationale explaining why each detection conclusion was formed. | [optional] 
**custom_policy_id** | **str** | Apply a Custom Policy for DLP Enforcement by providing the ID; to create a Custom Policy,  navigate to the Cloudmersive Management Portal and select Custom Policies.  Requires Managed Instance or Private Cloud | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


