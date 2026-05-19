# cloudmersive_dlp_api_client.TasksBatchJobApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**detect_audio_advanced_batch_job**](TasksBatchJobApi.md#detect_audio_advanced_batch_job) | **POST** /dlp/batch-job/detect/audio/advanced | Detect User Data in Audio File (Advanced) as a Batch Job
[**detect_audio_batch_job**](TasksBatchJobApi.md#detect_audio_batch_job) | **POST** /dlp/batch-job/detect/audio | Detect User Data in Audio File as a Batch Job
[**get_async_job_status**](TasksBatchJobApi.md#get_async_job_status) | **GET** /dlp/batch-job/status | Get the status and result of a DLP Batch Job
[**redact_audio_advanced_batch_job**](TasksBatchJobApi.md#redact_audio_advanced_batch_job) | **POST** /dlp/batch-job/redact/audio/advanced | Redact User Data in Audio File (Advanced) as a Batch Job
[**redact_audio_batch_job**](TasksBatchJobApi.md#redact_audio_batch_job) | **POST** /dlp/batch-job/redact/audio | Redact User Data in Audio File as a Batch Job


# **detect_audio_advanced_batch_job**
> DlpBatchJobResult detect_audio_advanced_batch_job(body=body)

Detect User Data in Audio File (Advanced) as a Batch Job

Creates an async batch job for detecting user data in an audio file using Advanced detection.  Use the GetAsyncJobStatus API to check on the status of the job and retrieve the result when complete.  Transcribes an audio file (WAV, MP3, M4A, FLAC, OGG, WMA) and detects 29 configurable types of user data including health-related PHI in the transcript using Advanced AI. Returns the full transcript, token timestamps, detection results, and optional rationale.  Requires Managed Instance or Private Cloud deployment.

### Example
```python
from __future__ import print_function
import time
import cloudmersive_dlp_api_client
from cloudmersive_dlp_api_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: Apikey
configuration = cloudmersive_dlp_api_client.Configuration()
configuration.api_key['Apikey'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Apikey'] = 'Bearer'

# create an instance of the API class
api_instance = cloudmersive_dlp_api_client.TasksBatchJobApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAdvancedAudioDetectionRequest() # DlpAdvancedAudioDetectionRequest | Input request (optional)

try:
    # Detect User Data in Audio File (Advanced) as a Batch Job
    api_response = api_instance.detect_audio_advanced_batch_job(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TasksBatchJobApi->detect_audio_advanced_batch_job: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAdvancedAudioDetectionRequest**](DlpAdvancedAudioDetectionRequest.md)| Input request | [optional] 

### Return type

[**DlpBatchJobResult**](DlpBatchJobResult.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detect_audio_batch_job**
> DlpBatchJobResult detect_audio_batch_job(body=body)

Detect User Data in Audio File as a Batch Job

Creates an async batch job for detecting user data in an audio file.  Use the GetAsyncJobStatus API to check on the status of the job and retrieve the result when complete.  Transcribes an audio file (WAV, MP3, M4A, FLAC, OGG, WMA) and detects 23 configurable types of user data in the transcript using Advanced AI. Returns the full transcript, token timestamps, and detection results.  Requires Managed Instance or Private Cloud deployment.

### Example
```python
from __future__ import print_function
import time
import cloudmersive_dlp_api_client
from cloudmersive_dlp_api_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: Apikey
configuration = cloudmersive_dlp_api_client.Configuration()
configuration.api_key['Apikey'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Apikey'] = 'Bearer'

# create an instance of the API class
api_instance = cloudmersive_dlp_api_client.TasksBatchJobApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAudioDetectionRequest() # DlpAudioDetectionRequest | Input request (optional)

try:
    # Detect User Data in Audio File as a Batch Job
    api_response = api_instance.detect_audio_batch_job(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TasksBatchJobApi->detect_audio_batch_job: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAudioDetectionRequest**](DlpAudioDetectionRequest.md)| Input request | [optional] 

### Return type

[**DlpBatchJobResult**](DlpBatchJobResult.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_async_job_status**
> DlpBatchJobStatusResult get_async_job_status(async_job_id=async_job_id)

Get the status and result of a DLP Batch Job

Returns the result of the Async Job - possible states can be STARTED or COMPLETED.  When COMPLETED, the corresponding result field (detection or redaction result) is populated on the response.  This API is only available for Cloudmersive Managed Instance and Private Cloud deployments.

### Example
```python
from __future__ import print_function
import time
import cloudmersive_dlp_api_client
from cloudmersive_dlp_api_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: Apikey
configuration = cloudmersive_dlp_api_client.Configuration()
configuration.api_key['Apikey'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Apikey'] = 'Bearer'

# create an instance of the API class
api_instance = cloudmersive_dlp_api_client.TasksBatchJobApi(cloudmersive_dlp_api_client.ApiClient(configuration))
async_job_id = 'async_job_id_example' # str | Job ID for the batch job to get the status of (optional)

try:
    # Get the status and result of a DLP Batch Job
    api_response = api_instance.get_async_job_status(async_job_id=async_job_id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TasksBatchJobApi->get_async_job_status: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **async_job_id** | **str**| Job ID for the batch job to get the status of | [optional] 

### Return type

[**DlpBatchJobStatusResult**](DlpBatchJobStatusResult.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **redact_audio_advanced_batch_job**
> DlpBatchJobResult redact_audio_advanced_batch_job(body=body)

Redact User Data in Audio File (Advanced) as a Batch Job

Creates an async batch job for redacting user data in an audio file using Advanced detection.  Use the GetAsyncJobStatus API to check on the status of the job and retrieve the redacted audio and transcript when complete.  Transcribes an audio file (WAV, MP3, M4A, FLAC, OGG, WMA), detects 34 configurable types of user data including health-related PHI in the transcript, and redacts audio segments containing PII. Returns the redacted audio, redacted transcript, detection results, redacted segment timestamps, and optional rationale.  Requires Managed Instance or Private Cloud deployment.

### Example
```python
from __future__ import print_function
import time
import cloudmersive_dlp_api_client
from cloudmersive_dlp_api_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: Apikey
configuration = cloudmersive_dlp_api_client.Configuration()
configuration.api_key['Apikey'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Apikey'] = 'Bearer'

# create an instance of the API class
api_instance = cloudmersive_dlp_api_client.TasksBatchJobApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAdvancedAudioRedactionRequest() # DlpAdvancedAudioRedactionRequest | Input request (optional)

try:
    # Redact User Data in Audio File (Advanced) as a Batch Job
    api_response = api_instance.redact_audio_advanced_batch_job(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TasksBatchJobApi->redact_audio_advanced_batch_job: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAdvancedAudioRedactionRequest**](DlpAdvancedAudioRedactionRequest.md)| Input request | [optional] 

### Return type

[**DlpBatchJobResult**](DlpBatchJobResult.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **redact_audio_batch_job**
> DlpBatchJobResult redact_audio_batch_job(body=body)

Redact User Data in Audio File as a Batch Job

Creates an async batch job for redacting user data in an audio file.  Use the GetAsyncJobStatus API to check on the status of the job and retrieve the redacted audio and transcript when complete.  Transcribes an audio file (WAV, MP3, M4A, FLAC, OGG, WMA), detects 23 configurable types of user data in the transcript, and redacts audio segments containing PII. Returns the redacted audio, redacted transcript, detection results, and redacted segment timestamps.  Requires Managed Instance or Private Cloud deployment.

### Example
```python
from __future__ import print_function
import time
import cloudmersive_dlp_api_client
from cloudmersive_dlp_api_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: Apikey
configuration = cloudmersive_dlp_api_client.Configuration()
configuration.api_key['Apikey'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Apikey'] = 'Bearer'

# create an instance of the API class
api_instance = cloudmersive_dlp_api_client.TasksBatchJobApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAudioRedactionRequest() # DlpAudioRedactionRequest | Input request (optional)

try:
    # Redact User Data in Audio File as a Batch Job
    api_response = api_instance.redact_audio_batch_job(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TasksBatchJobApi->redact_audio_batch_job: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAudioRedactionRequest**](DlpAudioRedactionRequest.md)| Input request | [optional] 

### Return type

[**DlpBatchJobResult**](DlpBatchJobResult.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

