# cloudmersive_dlp_api_client
Easily and directly scan and detect sensitive data (PII) in input text.

This Python package provides a native API client for [Cloudmersive DLP API](https://cloudmersive.com/dlp-data-loss-prevention-api)

- API version: v1
- Package version: 3.0.1
- Build package: io.swagger.codegen.languages.PythonClientCodegen

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on Github, you can install directly from Github

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import cloudmersive_dlp_api_client 
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import cloudmersive_dlp_api_client
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## Documentation for API Endpoints

All URIs are relative to *https://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DetectApi* | [**detect_document**](docs/DetectApi.md#detect_document) | **POST** /dlp/detect/document | Detect User Data in Document Image
*DetectApi* | [**detect_document_advanced**](docs/DetectApi.md#detect_document_advanced) | **POST** /dlp/detect/document/advanced | Detect User Data in Document Image (Advanced)
*DetectApi* | [**detect_text**](docs/DetectApi.md#detect_text) | **POST** /dlp/detect/text | Detect User Data in Input Text
*DetectApi* | [**detect_text_advanced**](docs/DetectApi.md#detect_text_advanced) | **POST** /dlp/detect/text/advanced | Detect User Data in Input Text (Advanced)
*RedactApi* | [**redact_document**](docs/RedactApi.md#redact_document) | **POST** /dlp/redact/document | Redact User Data in Document
*RedactApi* | [**redact_document_advanced**](docs/RedactApi.md#redact_document_advanced) | **POST** /dlp/redact/document/advanced | Redact User Data in Document (Advanced)
*RedactApi* | [**redact_text**](docs/RedactApi.md#redact_text) | **POST** /dlp/redact/text | Redact User Data in Input Text
*RedactApi* | [**redact_text_advanced**](docs/RedactApi.md#redact_text_advanced) | **POST** /dlp/redact/text/advanced | Redact User Data in Input Text (Advanced)


## Documentation For Models

 - [DlpAdvancedDetectionRequest](docs/DlpAdvancedDetectionRequest.md)
 - [DlpAdvancedDetectionResponse](docs/DlpAdvancedDetectionResponse.md)
 - [DlpAdvancedDocumentDetectionRequest](docs/DlpAdvancedDocumentDetectionRequest.md)
 - [DlpAdvancedDocumentRedactionRequest](docs/DlpAdvancedDocumentRedactionRequest.md)
 - [DlpAdvancedDocumentRedactionResponse](docs/DlpAdvancedDocumentRedactionResponse.md)
 - [DlpAdvancedRedactionRequest](docs/DlpAdvancedRedactionRequest.md)
 - [DlpAdvancedRedactionResponse](docs/DlpAdvancedRedactionResponse.md)
 - [DlpDetectionRequest](docs/DlpDetectionRequest.md)
 - [DlpDetectionResponse](docs/DlpDetectionResponse.md)
 - [DlpDocumentDetectionRequest](docs/DlpDocumentDetectionRequest.md)
 - [DlpDocumentRedactionRequest](docs/DlpDocumentRedactionRequest.md)
 - [DlpDocumentRedactionResponse](docs/DlpDocumentRedactionResponse.md)
 - [DlpRedactionRequest](docs/DlpRedactionRequest.md)
 - [DlpRedactionResponse](docs/DlpRedactionResponse.md)
 - [RedactedPageInfo](docs/RedactedPageInfo.md)


## Documentation For Authorization


## Apikey

- **Type**: API key
- **API key parameter name**: Apikey
- **Location**: HTTP header


## Author



