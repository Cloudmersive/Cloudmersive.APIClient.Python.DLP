# DlpBatchJobStatusResult

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**successful** | **bool** | True if the operation to check the status of the job was successful, false otherwise | [optional] 
**async_job_status** | **str** | Returns the job status of the Async Job, if applicable.  Possible states are STARTED and COMPLETED | [optional] 
**async_job_id** | **str** | Job ID | [optional] 
**detect_audio_result** | [**DlpAudioDetectionResponse**](DlpAudioDetectionResponse.md) |  | [optional] 
**detect_audio_advanced_result** | [**DlpAdvancedAudioDetectionResponse**](DlpAdvancedAudioDetectionResponse.md) |  | [optional] 
**redact_audio_result** | [**DlpAudioRedactionResponse**](DlpAudioRedactionResponse.md) |  | [optional] 
**redact_audio_advanced_result** | [**DlpAdvancedAudioRedactionResponse**](DlpAdvancedAudioRedactionResponse.md) |  | [optional] 
**error_message** | **str** | Error message (if any) | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


