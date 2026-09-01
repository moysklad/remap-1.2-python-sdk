# moysklad_remap_12_sdk.RetailSalesReturnsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_retail_sales_return**](RetailSalesReturnsApi.md#create_retail_sales_return) | **POST** /entity/retailsalesreturn | Создать Розничный возврат
[**create_retail_sales_return_metadata_attribute**](RetailSalesReturnsApi.md#create_retail_sales_return_metadata_attribute) | **POST** /entity/retailsalesreturn/metadata/attributes | Создать доп. поле Розничного возврата
[**create_retail_sales_return_position**](RetailSalesReturnsApi.md#create_retail_sales_return_position) | **POST** /entity/retailsalesreturn/{id}/positions | Создать и обновить позицию Розничного возврата
[**create_retail_sales_return_positions**](RetailSalesReturnsApi.md#create_retail_sales_return_positions) | **POST** /entity/retailsalesreturn/{id}/positions/batch | Массовое создание и обновление позиций Розничного возврата
[**create_retail_sales_returns_batch**](RetailSalesReturnsApi.md#create_retail_sales_returns_batch) | **POST** /entity/retailsalesreturn/batch | Создать или изменить Розничные возвраты
[**delete_retail_sales_return**](RetailSalesReturnsApi.md#delete_retail_sales_return) | **DELETE** /entity/retailsalesreturn/{id} | Удалить Розничный возврат
[**delete_retail_sales_return_metadata_attribute_by_id**](RetailSalesReturnsApi.md#delete_retail_sales_return_metadata_attribute_by_id) | **DELETE** /entity/retailsalesreturn/metadata/attributes/{id} | Удалить отдельное доп. поле Розничного возврата
[**delete_retail_sales_return_metadata_state_by_id**](RetailSalesReturnsApi.md#delete_retail_sales_return_metadata_state_by_id) | **DELETE** /entity/retailsalesreturn/metadata/states/{id} | Удалить отдельный статус Розничного возврата
[**delete_retail_sales_return_position**](RetailSalesReturnsApi.md#delete_retail_sales_return_position) | **DELETE** /entity/retailsalesreturn/{id}/positions/{positionId} | Удалить позицию Розничного возврата
[**delete_retail_sales_return_positions_batch**](RetailSalesReturnsApi.md#delete_retail_sales_return_positions_batch) | **POST** /entity/retailsalesreturn/{id}/positions/delete | Массовое удаление позиций Розничного возврата
[**get_retail_sales_return_by_id**](RetailSalesReturnsApi.md#get_retail_sales_return_by_id) | **GET** /entity/retailsalesreturn/{id} | Получить Розничный возврат
[**get_retail_sales_return_metadata**](RetailSalesReturnsApi.md#get_retail_sales_return_metadata) | **GET** /entity/retailsalesreturn/metadata | Метаданные Розничных возвратов
[**get_retail_sales_return_metadata_attribute**](RetailSalesReturnsApi.md#get_retail_sales_return_metadata_attribute) | **GET** /entity/retailsalesreturn/metadata/attributes | Доп. поля Розничного возврата
[**get_retail_sales_return_metadata_attribute_by_id**](RetailSalesReturnsApi.md#get_retail_sales_return_metadata_attribute_by_id) | **GET** /entity/retailsalesreturn/metadata/attributes/{id} | Отдельное доп. поле Розничного возврата
[**get_retail_sales_return_metadata_state_by_id**](RetailSalesReturnsApi.md#get_retail_sales_return_metadata_state_by_id) | **GET** /entity/retailsalesreturn/metadata/states/{id} | Отдельный статус Розничного возврата
[**get_retail_sales_return_position_by_id**](RetailSalesReturnsApi.md#get_retail_sales_return_position_by_id) | **GET** /entity/retailsalesreturn/{id}/positions/{positionId} | Получить позицию Розничного возврата
[**get_retail_sales_return_positions**](RetailSalesReturnsApi.md#get_retail_sales_return_positions) | **GET** /entity/retailsalesreturn/{id}/positions | Получить позиции Розничного возврата
[**get_retail_sales_return_template**](RetailSalesReturnsApi.md#get_retail_sales_return_template) | **PUT** /entity/retailsalesreturn/new | Шаблон Розничного возврата
[**get_retail_sales_returns**](RetailSalesReturnsApi.md#get_retail_sales_returns) | **GET** /entity/retailsalesreturn | Получить список Розничных возвратов
[**update_retail_sales_return**](RetailSalesReturnsApi.md#update_retail_sales_return) | **PUT** /entity/retailsalesreturn/{id} | Изменить Розничный возврат
[**update_retail_sales_return_metadata_attribute_by_id**](RetailSalesReturnsApi.md#update_retail_sales_return_metadata_attribute_by_id) | **PUT** /entity/retailsalesreturn/metadata/attributes/{id} | Обновить отдельное доп. поле Розничного возврата
[**update_retail_sales_return_metadata_state_by_id**](RetailSalesReturnsApi.md#update_retail_sales_return_metadata_state_by_id) | **PUT** /entity/retailsalesreturn/metadata/states/{id} | Обновить отдельный статус Розничного возврата
[**update_retail_sales_return_position**](RetailSalesReturnsApi.md#update_retail_sales_return_position) | **PUT** /entity/retailsalesreturn/{id}/positions/{positionId} | Изменить позицию Розничного возврата


# **create_retail_sales_return**
> RetailSalesReturn create_retail_sales_return(retail_sales_return, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать Розничный возврат

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return import RetailSalesReturn
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    retail_sales_return = moysklad_remap_12_sdk.RetailSalesReturn() # RetailSalesReturn | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать Розничный возврат
        api_response = api_instance.create_retail_sales_return(retail_sales_return, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->create_retail_sales_return:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->create_retail_sales_return: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **retail_sales_return** | [**RetailSalesReturn**](RetailSalesReturn.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**RetailSalesReturn**](RetailSalesReturn.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_retail_sales_return_metadata_attribute**
> AttributeMetaInfo create_retail_sales_return_metadata_attribute(attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать доп. поле Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.attribute_meta_info import AttributeMetaInfo
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    attribute_meta_info = moysklad_remap_12_sdk.AttributeMetaInfo() # AttributeMetaInfo | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать доп. поле Розничного возврата
        api_response = api_instance.create_retail_sales_return_metadata_attribute(attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->create_retail_sales_return_metadata_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->create_retail_sales_return_metadata_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attribute_meta_info** | [**AttributeMetaInfo**](AttributeMetaInfo.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**AttributeMetaInfo**](AttributeMetaInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_retail_sales_return_position**
> RetailSalesReturnPosition create_retail_sales_return_position(id, retail_sales_return_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать и обновить позицию Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return_position import RetailSalesReturnPosition
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    retail_sales_return_position = moysklad_remap_12_sdk.RetailSalesReturnPosition() # RetailSalesReturnPosition | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать и обновить позицию Розничного возврата
        api_response = api_instance.create_retail_sales_return_position(id, retail_sales_return_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->create_retail_sales_return_position:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->create_retail_sales_return_position: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **retail_sales_return_position** | [**RetailSalesReturnPosition**](RetailSalesReturnPosition.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**RetailSalesReturnPosition**](RetailSalesReturnPosition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_retail_sales_return_positions**
> List[CreateRetailSalesReturnPositions200ResponseInner] create_retail_sales_return_positions(id, retail_sales_return_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое создание и обновление позиций Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.create_retail_sales_return_positions200_response_inner import CreateRetailSalesReturnPositions200ResponseInner
from moysklad_remap_12_sdk.models.retail_sales_return_position import RetailSalesReturnPosition
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    retail_sales_return_position = [moysklad_remap_12_sdk.RetailSalesReturnPosition()] # List[RetailSalesReturnPosition] | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое создание и обновление позиций Розничного возврата
        api_response = api_instance.create_retail_sales_return_positions(id, retail_sales_return_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->create_retail_sales_return_positions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->create_retail_sales_return_positions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **retail_sales_return_position** | [**List[RetailSalesReturnPosition]**](RetailSalesReturnPosition.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[CreateRetailSalesReturnPositions200ResponseInner]**](CreateRetailSalesReturnPositions200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_retail_sales_returns_batch**
> List[CreateRetailSalesReturnsBatch200ResponseInner] create_retail_sales_returns_batch(retail_sales_return, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать или изменить Розничные возвраты

Создание или изменение нескольких Розничных возвратов.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.create_retail_sales_returns_batch200_response_inner import CreateRetailSalesReturnsBatch200ResponseInner
from moysklad_remap_12_sdk.models.retail_sales_return import RetailSalesReturn
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    retail_sales_return = [moysklad_remap_12_sdk.RetailSalesReturn()] # List[RetailSalesReturn] | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать или изменить Розничные возвраты
        api_response = api_instance.create_retail_sales_returns_batch(retail_sales_return, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->create_retail_sales_returns_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->create_retail_sales_returns_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **retail_sales_return** | [**List[RetailSalesReturn]**](RetailSalesReturn.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[CreateRetailSalesReturnsBatch200ResponseInner]**](CreateRetailSalesReturnsBatch200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Розничные возвраты успешно созданы или изменены |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_retail_sales_return**
> delete_retail_sales_return(id, accept=accept, accept_encoding=accept_encoding)

Удалить Розничный возврат

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить Розничный возврат
        api_instance.delete_retail_sales_return(id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->delete_retail_sales_return: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_retail_sales_return_metadata_attribute_by_id**
> delete_retail_sales_return_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding)

Удалить отдельное доп. поле Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить отдельное доп. поле Розничного возврата
        api_instance.delete_retail_sales_return_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->delete_retail_sales_return_metadata_attribute_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_retail_sales_return_metadata_state_by_id**
> delete_retail_sales_return_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding)

Удалить отдельный статус Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить отдельный статус Розничного возврата
        api_instance.delete_retail_sales_return_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->delete_retail_sales_return_metadata_state_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**404** | Запрошенный ресурс не существует (тело ответа отсутствует) |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_retail_sales_return_position**
> delete_retail_sales_return_position(id, position_id, expand=expand, accept=accept, accept_encoding=accept_encoding)

Удалить позицию Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    position_id = 'position_id_example' # str | ID позиции
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить позицию Розничного возврата
        api_instance.delete_retail_sales_return_position(id, position_id, expand=expand, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->delete_retail_sales_return_position: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **position_id** | **str**| ID позиции | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_retail_sales_return_positions_batch**
> List[DeleteInvoiceOutBatch200ResponseInner] delete_retail_sales_return_positions_batch(id, retail_sales_return_position, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое удаление позиций Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.delete_invoice_out_batch200_response_inner import DeleteInvoiceOutBatch200ResponseInner
from moysklad_remap_12_sdk.models.retail_sales_return_position import RetailSalesReturnPosition
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    retail_sales_return_position = [moysklad_remap_12_sdk.RetailSalesReturnPosition()] # List[RetailSalesReturnPosition] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое удаление позиций Розничного возврата
        api_response = api_instance.delete_retail_sales_return_positions_batch(id, retail_sales_return_position, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->delete_retail_sales_return_positions_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->delete_retail_sales_return_positions_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **retail_sales_return_position** | [**List[RetailSalesReturnPosition]**](RetailSalesReturnPosition.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[DeleteInvoiceOutBatch200ResponseInner]**](DeleteInvoiceOutBatch200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Результат по каждому элементу (успех или объект ошибки) |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_by_id**
> RetailSalesReturn get_retail_sales_return_by_id(id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)

Получить Розничный возврат

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return import RetailSalesReturn
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Розничный возврат
        api_response = api_instance.get_retail_sales_return_by_id(id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**RetailSalesReturn**](RetailSalesReturn.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_metadata**
> DocumentMetadata get_retail_sales_return_metadata(accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Метаданные Розничных возвратов

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.document_metadata import DocumentMetadata
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Метаданные Розничных возвратов
        api_response = api_instance.get_retail_sales_return_metadata(accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**DocumentMetadata**](DocumentMetadata.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_metadata_attribute**
> AttributeMetaInfoList get_retail_sales_return_metadata_attribute(offset=offset, limit=limit, accept=accept, accept_encoding=accept_encoding)

Доп. поля Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.attribute_meta_info_list import AttributeMetaInfoList
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Доп. поля Розничного возврата
        api_response = api_instance.get_retail_sales_return_metadata_attribute(offset=offset, limit=limit, accept=accept, accept_encoding=accept_encoding)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_metadata_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_metadata_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**AttributeMetaInfoList**](AttributeMetaInfoList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_metadata_attribute_by_id**
> AttributeMetaInfo get_retail_sales_return_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding)

Отдельное доп. поле Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.attribute_meta_info import AttributeMetaInfo
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Отдельное доп. поле Розничного возврата
        api_response = api_instance.get_retail_sales_return_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_metadata_attribute_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_metadata_attribute_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**AttributeMetaInfo**](AttributeMetaInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_metadata_state_by_id**
> State get_retail_sales_return_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding)

Отдельный статус Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.state import State
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Отдельный статус Розничного возврата
        api_response = api_instance.get_retail_sales_return_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_metadata_state_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_metadata_state_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**State**](State.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_position_by_id**
> RetailSalesReturnPosition get_retail_sales_return_position_by_id(id, position_id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)

Получить позицию Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return_position import RetailSalesReturnPosition
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    position_id = 'position_id_example' # str | ID позиции
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить позицию Розничного возврата
        api_response = api_instance.get_retail_sales_return_position_by_id(id, position_id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_position_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_position_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **position_id** | **str**| ID позиции | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**RetailSalesReturnPosition**](RetailSalesReturnPosition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_positions**
> RetailSalesReturnPositionList get_retail_sales_return_positions(id, limit=limit, offset=offset, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)

Получить позиции Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return_position_list import RetailSalesReturnPositionList
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить позиции Розничного возврата
        api_response = api_instance.get_retail_sales_return_positions(id, limit=limit, offset=offset, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_positions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_positions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**RetailSalesReturnPositionList**](RetailSalesReturnPositionList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_return_template**
> RetailSalesReturn get_retail_sales_return_template(accept=accept, accept_encoding=accept_encoding, content_type=content_type, body=body)

Шаблон Розничного возврата

Предзаполненный шаблон Розничного возврата.
В теле запроса можно передать `retailShift` для шаблона без основания или `demand` для шаблона на основе Розничной продажи.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return import RetailSalesReturn
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)
    body = None # object |  (optional)

    try:
        # Шаблон Розничного возврата
        api_response = api_instance.get_retail_sales_return_template(accept=accept, accept_encoding=accept_encoding, content_type=content_type, body=body)
        print("The response of RetailSalesReturnsApi->get_retail_sales_return_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_return_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]
 **body** | **object**|  | [optional] 

### Return type

[**RetailSalesReturn**](RetailSalesReturn.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_retail_sales_returns**
> RetailSalesReturnList get_retail_sales_returns(limit=limit, offset=offset, search=search, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)

Получить список Розничных возвратов

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return_list import RetailSalesReturnList
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    search = 'search_example' # str | Контекстный поиск по строковым полям сущностей (optional)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить список Розничных возвратов
        api_response = api_instance.get_retail_sales_returns(limit=limit, offset=offset, search=search, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)
        print("The response of RetailSalesReturnsApi->get_retail_sales_returns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->get_retail_sales_returns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **search** | **str**| Контекстный поиск по строковым полям сущностей | [optional] 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**RetailSalesReturnList**](RetailSalesReturnList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_retail_sales_return**
> RetailSalesReturn update_retail_sales_return(id, retail_sales_return, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Изменить Розничный возврат

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return import RetailSalesReturn
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    retail_sales_return = moysklad_remap_12_sdk.RetailSalesReturn() # RetailSalesReturn | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Изменить Розничный возврат
        api_response = api_instance.update_retail_sales_return(id, retail_sales_return, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->update_retail_sales_return:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->update_retail_sales_return: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **retail_sales_return** | [**RetailSalesReturn**](RetailSalesReturn.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**RetailSalesReturn**](RetailSalesReturn.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_retail_sales_return_metadata_attribute_by_id**
> AttributeMetaInfo update_retail_sales_return_metadata_attribute_by_id(id, attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить отдельное доп. поле Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.attribute_meta_info import AttributeMetaInfo
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    attribute_meta_info = moysklad_remap_12_sdk.AttributeMetaInfo() # AttributeMetaInfo | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить отдельное доп. поле Розничного возврата
        api_response = api_instance.update_retail_sales_return_metadata_attribute_by_id(id, attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->update_retail_sales_return_metadata_attribute_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->update_retail_sales_return_metadata_attribute_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **attribute_meta_info** | [**AttributeMetaInfo**](AttributeMetaInfo.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**AttributeMetaInfo**](AttributeMetaInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_retail_sales_return_metadata_state_by_id**
> State update_retail_sales_return_metadata_state_by_id(id, state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить отдельный статус Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.state import State
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    state = moysklad_remap_12_sdk.State() # State | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить отдельный статус Розничного возврата
        api_response = api_instance.update_retail_sales_return_metadata_state_by_id(id, state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->update_retail_sales_return_metadata_state_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->update_retail_sales_return_metadata_state_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **state** | [**State**](State.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**State**](State.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_retail_sales_return_position**
> RetailSalesReturnPosition update_retail_sales_return_position(id, position_id, retail_sales_return_position, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Изменить позицию Розничного возврата

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.retail_sales_return_position import RetailSalesReturnPosition
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
    api_instance = moysklad_remap_12_sdk.RetailSalesReturnsApi(api_client)
    id = 'id_example' # str | ID сущности
    position_id = 'position_id_example' # str | ID позиции
    retail_sales_return_position = moysklad_remap_12_sdk.RetailSalesReturnPosition() # RetailSalesReturnPosition | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Изменить позицию Розничного возврата
        api_response = api_instance.update_retail_sales_return_position(id, position_id, retail_sales_return_position, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of RetailSalesReturnsApi->update_retail_sales_return_position:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RetailSalesReturnsApi->update_retail_sales_return_position: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **position_id** | **str**| ID позиции | 
 **retail_sales_return_position** | [**RetailSalesReturnPosition**](RetailSalesReturnPosition.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**RetailSalesReturnPosition**](RetailSalesReturnPosition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

