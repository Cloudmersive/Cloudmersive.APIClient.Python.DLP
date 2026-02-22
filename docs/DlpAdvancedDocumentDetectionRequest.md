# DlpAdvancedDocumentDetectionRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input_file** | **str** | Document file bytes (PDF, DOCX, PNG, or JPG) to scan for PII and sensitive data. | [optional] 
**file_name** | **str** | Optional. Name of the input file including extension, used for format detection. If not provided, format is detected from file contents. | [optional] 
**recognition_mode** | **str** | Optional. Recognition mode for image processing. Options: null (default), \&quot;Fast\&quot;, \&quot;FastPlus\&quot;, \&quot;FastMini\&quot;. | [optional] 
**allow_email_address** | **bool** | Set to true to allow email addresses in the document and not flag them as PII. | [optional] 
**allow_phone_number** | **bool** | Set to true to allow phone numbers in the document and not flag them as PII. | [optional] 
**allow_street_address** | **bool** | Set to true to allow street addresses in the document and not flag them as PII. | [optional] 
**allow_person_name** | **bool** | Set to true to allow person names in the document and not flag them as PII. | [optional] 
**allow_birth_date** | **bool** | Set to true to allow birth dates in the document and not flag them as PII. | [optional] 
**allow_passport_number** | **bool** | Set to true to allow passport numbers in the document and not flag them as PII. | [optional] 
**allow_drivers_license** | **bool** | Set to true to allow drivers license numbers in the document and not flag them as PII. | [optional] 
**allow_social_security_number** | **bool** | Set to true to allow social security numbers in the document and not flag them as PII. | [optional] 
**allow_taxpayer_id** | **bool** | Set to true to allow taxpayer IDs in the document and not flag them as PII. | [optional] 
**allow_credit_card_number** | **bool** | Set to true to allow credit card numbers in the document and not flag them as PII. | [optional] 
**allow_credit_card_expiration_date** | **bool** | Set to true to allow credit card expiration dates in the document and not flag them as PII. | [optional] 
**allow_credit_card_verification_code** | **bool** | Set to true to allow credit card verification codes in the document and not flag them as PII. | [optional] 
**allow_bank_account_number** | **bool** | Set to true to allow bank account numbers in the document and not flag them as PII. | [optional] 
**allow_iban** | **bool** | Set to true to allow IBANs in the document and not flag them as PII. | [optional] 
**allow_health_insurance_number** | **bool** | Set to true to allow health insurance numbers in the document and not flag them as PII. | [optional] 
**allow_bearer_token** | **bool** | Set to true to allow bearer tokens in the document and not flag them as PII. | [optional] 
**allow_http_cookie** | **bool** | Set to true to allow HTTP cookies in the document and not flag them as PII. | [optional] 
**allow_private_keys** | **bool** | Set to true to allow private keys in the document and not flag them as PII. | [optional] 
**allow_credentials** | **bool** | Set to true to allow credentials (usernames/passwords) in the document and not flag them as PII. | [optional] 
**allow_deep_web_urls** | **bool** | Set to true to allow deep web URLs (.onion) in the document and not flag them as PII. | [optional] 
**allow_source_code** | **bool** | Set to true to allow source code in the document and not flag it as sensitive data. | [optional] 
**allow_ip_address** | **bool** | Set to true to allow IP addresses in the document and not flag them as PII. | [optional] 
**allow_mac_address** | **bool** | Set to true to allow MAC addresses in the document and not flag them as PII. | [optional] 
**allow_health_insurance_member_id** | **bool** | Set to true to allow health insurance member IDs in the document and not flag them as PHI. | [optional] 
**allow_health_injury_or_disease** | **bool** | Set to true to allow references to injuries or diseases in the document and not flag them as PHI. | [optional] 
**allow_health_type_of_treatment** | **bool** | Set to true to allow references to types of medical treatment in the document and not flag them as PHI. | [optional] 
**allow_health_date_and_time_of_treatment** | **bool** | Set to true to allow dates and times of medical treatment in the document and not flag them as PHI. | [optional] 
**allow_health_plan_beneficiary_number** | **bool** | Set to true to allow health plan beneficiary numbers in the document and not flag them as PHI. | [optional] 
**allow_health_payments_made_for_treatment** | **bool** | Set to true to allow payments made for medical treatment in the document and not flag them as PHI. | [optional] 
**allow_faces** | **bool** | Set to true to allow identifiable human faces in the document and not flag them as PII. | [optional] 
**allow_vehicle_id** | **bool** | Set to true to allow vehicle identifiers (e.g. license plates, VINs) in the document and not flag them as PII. | [optional] 
**allow_device_id** | **bool** | Set to true to allow device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs) in the document and not flag them as PII. | [optional] 
**allow_names_of_relatives** | **bool** | Set to true to allow names of relatives in the document and not flag them as PII. | [optional] 
**allow_health_universal_record_locator** | **bool** | Set to true to allow health universal record locators (URLs) in the document and not flag them as PHI. | [optional] 
**allow_biometrics** | **bool** | Set to true to allow biometric data references (e.g. fingerprints, retinal scans, voiceprints) in the document and not flag them as PII. | [optional] 
**provide_analysis_rationale** | **bool** | Set to true to include a natural language rationale explaining why each detection conclusion was formed. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


