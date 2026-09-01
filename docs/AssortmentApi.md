# moysklad_remap_12_sdk.AssortmentApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_assortment_positions_batch**](AssortmentApi.md#delete_assortment_positions_batch) | **POST** /entity/assortment/delete | Удалить позиции ассортимента
[**get_assortment**](AssortmentApi.md#get_assortment) | **GET** /entity/assortment | Получить список ассортимента
[**get_assortment_settings**](AssortmentApi.md#get_assortment_settings) | **GET** /entity/assortment/settings | Получить настройки ассортимента
[**update_assortment_settings**](AssortmentApi.md#update_assortment_settings) | **PUT** /entity/assortment/settings | Изменить настройки ассортимента


# **delete_assortment_positions_batch**
> List[DeleteRowResult] delete_assortment_positions_batch(assortment, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить позиции ассортимента

Массовое удаление позиций в Ассортименте

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.assortment import Assortment
from moysklad_remap_12_sdk.models.delete_row_result import DeleteRowResult
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
    api_instance = moysklad_remap_12_sdk.AssortmentApi(api_client)
    assortment = [moysklad_remap_12_sdk.Assortment()] # List[Assortment] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить позиции ассортимента
        api_response = api_instance.delete_assortment_positions_batch(assortment, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of AssortmentApi->delete_assortment_positions_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AssortmentApi->delete_assortment_positions_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assortment** | [**List[Assortment]**](Assortment.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[DeleteRowResult]**](DeleteRowResult.md)

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

# **get_assortment**
> AssortmentList get_assortment(limit=limit, offset=offset, search=search, filter=filter, expand=expand, order=order, group_by=group_by, stock_mode=stock_mode, quantity_mode=quantity_mode, accept=accept, accept_encoding=accept_encoding)

Получить список ассортимента

Запрос всех товаров, услуг, комплектов, модификаций и партий в виде списка

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.assortment_list import AssortmentList
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
    api_instance = moysklad_remap_12_sdk.AssortmentApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    search = 'search_example' # str | Контекстный поиск по строковым полям сущностей (optional)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    order = 'order_example' # str | Сортировка (optional)
    group_by = 'group_by_example' # str | Параметр группировки (product, variant, consignment) (optional)
    stock_mode = 'stock_mode_example' # str | Фильтрация по значению остатка (optional)
    quantity_mode = 'quantity_mode_example' # str | Фильтрация по значению доступно (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить список ассортимента
        api_response = api_instance.get_assortment(limit=limit, offset=offset, search=search, filter=filter, expand=expand, order=order, group_by=group_by, stock_mode=stock_mode, quantity_mode=quantity_mode, accept=accept, accept_encoding=accept_encoding)
        print("The response of AssortmentApi->get_assortment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AssortmentApi->get_assortment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **search** | **str**| Контекстный поиск по строковым полям сущностей | [optional] 
 **filter** | **str**| Фильтрация выборки | [optional] 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **order** | **str**| Сортировка | [optional] 
 **group_by** | **str**| Параметр группировки (product, variant, consignment) | [optional] 
 **stock_mode** | **str**| Фильтрация по значению остатка | [optional] 
 **quantity_mode** | **str**| Фильтрация по значению доступно | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**AssortmentList**](AssortmentList.md)

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

# **get_assortment_settings**
> AssortmentSettings get_assortment_settings(accept=accept, accept_encoding=accept_encoding)

Получить настройки ассортимента

Запрос на получение настроек справочника товаров

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.assortment_settings import AssortmentSettings
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
    api_instance = moysklad_remap_12_sdk.AssortmentApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить настройки ассортимента
        api_response = api_instance.get_assortment_settings(accept=accept, accept_encoding=accept_encoding)
        print("The response of AssortmentApi->get_assortment_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AssortmentApi->get_assortment_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**AssortmentSettings**](AssortmentSettings.md)

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

# **update_assortment_settings**
> AssortmentSettings update_assortment_settings(assortment_settings, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Изменить настройки ассортимента

Запрос на изменение настроек справочника товаров

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.assortment_settings import AssortmentSettings
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
    api_instance = moysklad_remap_12_sdk.AssortmentApi(api_client)
    assortment_settings = moysklad_remap_12_sdk.AssortmentSettings() # AssortmentSettings | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Изменить настройки ассортимента
        api_response = api_instance.update_assortment_settings(assortment_settings, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of AssortmentApi->update_assortment_settings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AssortmentApi->update_assortment_settings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assortment_settings** | [**AssortmentSettings**](AssortmentSettings.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**AssortmentSettings**](AssortmentSettings.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Настройки ассортимента успешно обновлены |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

