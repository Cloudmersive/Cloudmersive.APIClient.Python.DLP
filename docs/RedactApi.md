# cloudmersive_dlp_api_client.RedactApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**redact_document**](RedactApi.md#redact_document) | **POST** /dlp/redact/document | Redact User Data in Document
[**redact_document_advanced**](RedactApi.md#redact_document_advanced) | **POST** /dlp/redact/document/advanced | Redact User Data in Document (Advanced)
[**redact_text**](RedactApi.md#redact_text) | **POST** /dlp/redact/text | Redact User Data in Input Text
[**redact_text_advanced**](RedactApi.md#redact_text_advanced) | **POST** /dlp/redact/text/advanced | Redact User Data in Input Text (Advanced)


# **redact_document**
> DlpDocumentRedactionResponse redact_document(body=body)

Redact User Data in Document

Detects and redacts configurable types of user data in a document (PDF, DOCX, PNG, JPG) using Advanced AI. Rasterizes document pages, detects PII regions using a grid-overlay approach, blurs those regions, and returns a rasterized PDF.

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
api_instance = cloudmersive_dlp_api_client.RedactApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpDocumentRedactionRequest() # DlpDocumentRedactionRequest | Input request (optional)

try:
    # Redact User Data in Document
    api_response = api_instance.redact_document(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling RedactApi->redact_document: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpDocumentRedactionRequest**](DlpDocumentRedactionRequest.md)| Input request | [optional] 

### Return type

[**DlpDocumentRedactionResponse**](DlpDocumentRedactionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **redact_document_advanced**
> DlpAdvancedDocumentRedactionResponse redact_document_advanced(body=body)

Redact User Data in Document (Advanced)

Detects and redacts 35 configurable types of user data including health-related PHI in a document (PDF, DOCX, PNG, JPG) using Advanced AI. Rasterizes document pages, detects PII regions using a row-overlay approach, redacts those regions, and returns a rasterized PDF.

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
api_instance = cloudmersive_dlp_api_client.RedactApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAdvancedDocumentRedactionRequest() # DlpAdvancedDocumentRedactionRequest | Input request (optional)

try:
    # Redact User Data in Document (Advanced)
    api_response = api_instance.redact_document_advanced(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling RedactApi->redact_document_advanced: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAdvancedDocumentRedactionRequest**](DlpAdvancedDocumentRedactionRequest.md)| Input request | [optional] 

### Return type

[**DlpAdvancedDocumentRedactionResponse**](DlpAdvancedDocumentRedactionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **redact_text**
> DlpRedactionResponse redact_text(body=body)

Redact User Data in Input Text

Detects and redacts configurable types of user data in an input text string using Advanced AI. First detects PII, then redacts disallowed types by either deleting them or replacing them with asterisks.

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
api_instance = cloudmersive_dlp_api_client.RedactApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpRedactionRequest() # DlpRedactionRequest | Input request (optional)

try:
    # Redact User Data in Input Text
    api_response = api_instance.redact_text(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling RedactApi->redact_text: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpRedactionRequest**](DlpRedactionRequest.md)| Input request | [optional] 

### Return type

[**DlpRedactionResponse**](DlpRedactionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **redact_text_advanced**
> DlpAdvancedRedactionResponse redact_text_advanced(body=body)

Redact User Data in Input Text (Advanced)

Detects and redacts 34 configurable types of user data including health-related PHI in an input text string using Advanced AI. First detects PII, then redacts disallowed types by either deleting them or replacing them with asterisks.

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
api_instance = cloudmersive_dlp_api_client.RedactApi(cloudmersive_dlp_api_client.ApiClient(configuration))
body = cloudmersive_dlp_api_client.DlpAdvancedRedactionRequest() # DlpAdvancedRedactionRequest | Input request (optional)

try:
    # Redact User Data in Input Text (Advanced)
    api_response = api_instance.redact_text_advanced(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling RedactApi->redact_text_advanced: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**DlpAdvancedRedactionRequest**](DlpAdvancedRedactionRequest.md)| Input request | [optional] 

### Return type

[**DlpAdvancedRedactionResponse**](DlpAdvancedRedactionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

