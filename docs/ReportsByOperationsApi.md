# moysklad_remap_12_sdk.ReportsByOperationsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_by_operations_in_transit**](ReportsByOperationsApi.md#get_by_operations_in_transit) | **GET** /report/byoperations/intransit | Получить Отчет по документам, отображающий ожидание
[**get_by_operations_reserve**](ReportsByOperationsApi.md#get_by_operations_reserve) | **GET** /report/byoperations/reserve | Получить Отчет по документам, отображающий резервы
[**get_by_operations_stock**](ReportsByOperationsApi.md#get_by_operations_stock) | **GET** /report/byoperations/stock | Получить Отчет по документам, отображающий остатки


# **get_by_operations_in_transit**
> ByOperationsInTransitList get_by_operations_in_transit(filter, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)

Получить Отчет по документам, отображающий ожидание

Отчет по документам номенклатуры, формирующим ожидания.
Обязательный параметр фильтрации — `filter` с полем `assortment`
(ссылка на товар, модификацию или партию; только одна номенклатура).
Для доступа нужны права на просмотр товаров и остатков.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.by_operations_in_transit_list import ByOperationsInTransitList
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
    api_instance = moysklad_remap_12_sdk.ReportsByOperationsApi(api_client)
    filter = 'filter_example' # str | Фильтрация выборки. Обязательно указать `assortment=<href>` — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре. 
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Отчет по документам, отображающий ожидание
        api_response = api_instance.get_by_operations_in_transit(filter, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsByOperationsApi->get_by_operations_in_transit:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsByOperationsApi->get_by_operations_in_transit: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **str**| Фильтрация выборки. Обязательно указать &#x60;assortment&#x3D;&lt;href&gt;&#x60; — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре.  | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ByOperationsInTransitList**](ByOperationsInTransitList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_by_operations_reserve**
> ByOperationsReserveList get_by_operations_reserve(filter, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)

Получить Отчет по документам, отображающий резервы

Отчет по документам номенклатуры, формирующим резервы.
Обязательный параметр фильтрации — `filter` с полем `assortment`
(ссылка на товар, модификацию или партию; только одна номенклатура).
Для доступа нужны права на просмотр товаров и остатков.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.by_operations_reserve_list import ByOperationsReserveList
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
    api_instance = moysklad_remap_12_sdk.ReportsByOperationsApi(api_client)
    filter = 'filter_example' # str | Фильтрация выборки. Обязательно указать `assortment=<href>` — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре. 
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Отчет по документам, отображающий резервы
        api_response = api_instance.get_by_operations_reserve(filter, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsByOperationsApi->get_by_operations_reserve:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsByOperationsApi->get_by_operations_reserve: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **str**| Фильтрация выборки. Обязательно указать &#x60;assortment&#x3D;&lt;href&gt;&#x60; — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре.  | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ByOperationsReserveList**](ByOperationsReserveList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_by_operations_stock**
> ByOperationsStockList get_by_operations_stock(filter, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)

Получить Отчет по документам, отображающий остатки

Отчет по документам номенклатуры, формирующим остатки.
Обязательный параметр фильтрации — `filter` с полем `assortment`
(ссылка на товар, модификацию или партию; только одна номенклатура).
Для доступа нужны права на просмотр товаров и остатков.
Поля себестоимости (`costPerUnit`, `sumCost`) не возвращаются без пермиссии
«Видеть себестоимость, цену закупки, прибыль товаров».


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.by_operations_stock_list import ByOperationsStockList
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
    api_instance = moysklad_remap_12_sdk.ReportsByOperationsApi(api_client)
    filter = 'filter_example' # str | Фильтрация выборки. Обязательно указать `assortment=<href>` — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре. 
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Отчет по документам, отображающий остатки
        api_response = api_instance.get_by_operations_stock(filter, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsByOperationsApi->get_by_operations_stock:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsByOperationsApi->get_by_operations_stock: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **str**| Фильтрация выборки. Обязательно указать &#x60;assortment&#x3D;&lt;href&gt;&#x60; — ссылку на товар, модификацию или партию. Можно фильтровать только по одной номенклатуре.  | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ByOperationsStockList**](ByOperationsStockList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

