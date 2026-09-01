# moysklad_remap_12_sdk.LabelsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**print_labels**](LabelsApi.md#print_labels) | **POST** /entity/{type}/{id}/export | Запрос на печать этикеток и ценников


# **print_labels**
> print_labels(id, type, label_print_request, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Запрос на печать этикеток и ценников

Запрос на формирование печатной формы с этикетками и ценниками.
В случае готовности сервер возвращает пустой ответ с кодом 303 и заголовком Location.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.label_print_request import LabelPrintRequest
from moysklad_remap_12_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.moysklad.ru/api/remap/1.2
# See configuration.py for a list of all supported configuration parameters.
configuration = moysklad_remap_12_sdk.Configuration(
    host = "https://api.moysklad.ru/api/remap/1.2"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = moysklad_remap_12_sdk.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Configure Bearer authorization: bearerAuth
configuration = moysklad_remap_12_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with moysklad_remap_12_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moysklad_remap_12_sdk.LabelsApi(api_client)
    id = 'id_example' # str | ID сущности
    type = 'type_example' # str | Тип сущности, для которой запрашивается печать
    label_print_request = moysklad_remap_12_sdk.LabelPrintRequest() # LabelPrintRequest | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Запрос на печать этикеток и ценников
        api_instance.print_labels(id, type, label_print_request, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling LabelsApi->print_labels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **type** | **str**| Тип сущности, для которой запрашивается печать | 
 **label_print_request** | [**LabelPrintRequest**](LabelPrintRequest.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Печатная форма еще не готова, в Location передана ссылка на статус печати |  * Location - Ссылка на статус печати <br>  * Content-Type - Тип содержимого ответа <br>  |
**303** | Печатная форма готова, в Location передана ссылка на файл |  * Location - Ссылка на статус печати <br>  * Content-Type - Тип содержимого ответа <br>  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

