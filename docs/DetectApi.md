# cloudmersive_dlp_api_client.DetectApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**detect_document**](DetectApi.md#detect_document) | **POST** /dlp/detect/document | Detect User Data in Document Image
[**detect_document_advanced**](DetectApi.md#detect_document_advanced) | **POST** /dlp/detect/document/advanced | Detect User Data in Document Image (Advanced)
[**detect_text**](DetectApi.md#detect_text) | **POST** /dlp/detect/text | Detect User Data in Input Text
[**detect_text_advanced**](DetectApi.md#detect_text_advanced) | **POST** /dlp/detect/text/advanced | Detect User Data in Input Text (Advanced)


# **detect_document**
> DlpDetectionResponse detect_document(body=body)

Detect User Data in Document Image

Detects configurable types of user data in a document (PDF, DOC, DOCX, XLS, XLSX, PPT, PPTX, HTML, EML, MSG, PNG, JPG, WEBP) using Advanced AI.

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
api_instance = cloudmersive_dlp_api_client.DetectApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpDocumentDetectionRequest() # DlpDocumentDetectionRequest | Input request (optional)

try:
    # Detect User Data in Document Image
    api_response = api_instance.detect_document(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DetectApi->detect_document: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpDocumentDetectionRequest**](DlpDocumentDetectionRequest.md)| Input request | [optional] 

### Return type

[**DlpDetectionResponse**](DlpDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detect_document_advanced**
> DlpAdvancedDetectionResponse detect_document_advanced(body=body)

Detect User Data in Document Image (Advanced)

Detects 29 configurable types of user data including health-related PHI in a document (PDF, DOC, DOCX, XLS, XLSX, PPT, PPTX, HTML, EML, MSG, PNG, JPG, WEBP) using Advanced AI.

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
api_instance = cloudmersive_dlp_api_client.DetectApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAdvancedDocumentDetectionRequest() # DlpAdvancedDocumentDetectionRequest | Input request (optional)

try:
    # Detect User Data in Document Image (Advanced)
    api_response = api_instance.detect_document_advanced(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DetectApi->detect_document_advanced: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAdvancedDocumentDetectionRequest**](DlpAdvancedDocumentDetectionRequest.md)| Input request | [optional] 

### Return type

[**DlpAdvancedDetectionResponse**](DlpAdvancedDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detect_text**
> DlpDetectionResponse detect_text(body=body)

Detect User Data in Input Text

Detects configurable types of user data in an input text string using Advanced AI.

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
api_instance = cloudmersive_dlp_api_client.DetectApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpDetectionRequest() # DlpDetectionRequest | Input request (optional)

try:
    # Detect User Data in Input Text
    api_response = api_instance.detect_text(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DetectApi->detect_text: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpDetectionRequest**](DlpDetectionRequest.md)| Input request | [optional] 

### Return type

[**DlpDetectionResponse**](DlpDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detect_text_advanced**
> DlpAdvancedDetectionResponse detect_text_advanced(body=body)

Detect User Data in Input Text (Advanced)

Detects 29 configurable types of user data including health-related PHI in an input text string using Advanced AI.

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
api_instance = cloudmersive_dlp_api_client.DetectApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAdvancedDetectionRequest() # DlpAdvancedDetectionRequest | Input request (optional)

try:
    # Detect User Data in Input Text (Advanced)
    api_response = api_instance.detect_text_advanced(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DetectApi->detect_text_advanced: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAdvancedDetectionRequest**](DlpAdvancedDetectionRequest.md)| Input request | [optional] 

### Return type

[**DlpAdvancedDetectionResponse**](DlpAdvancedDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

