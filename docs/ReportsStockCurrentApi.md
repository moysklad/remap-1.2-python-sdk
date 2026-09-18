# moysklad_remap_12_sdk.ReportsStockCurrentApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_stock_all_current**](ReportsStockCurrentApi.md#get_stock_all_current) | **GET** /report/stock/all/current | Получить Краткий отчет об остатках
[**get_stock_by_slot_current**](ReportsStockCurrentApi.md#get_stock_by_slot_current) | **GET** /report/stock/byslot/current | Получить Краткий отчет об остатках по ячейкам
[**get_stock_by_store_current**](ReportsStockCurrentApi.md#get_stock_by_store_current) | **GET** /report/stock/bystore/current | Получить Краткий отчет об остатках по складам


# **get_stock_all_current**
> List[StockCurrentAll] get_stock_all_current(include=include, changed_since=changed_since, stock_type=stock_type, filter=filter, accept=accept, accept_encoding=accept_encoding)

Получить Краткий отчет об остатках

Краткий отчет об остатках для частого обновления данных по номенклатуре.
Возвращает один тип значения остатка, выбранный параметром `stockType`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.stock_current_all import StockCurrentAll
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
    api_instance = moysklad_remap_12_sdk.ReportsStockCurrentApi(api_client)
    include = 'include_example' # str | Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  (optional)
    changed_since = 'changed_since_example' # str | Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: `yyyy-MM-dd HH:mm:ss`.  (optional)
    stock_type = stock # str | Тип рассчитываемого значения остатка. По умолчанию `stock`.  (optional) (default to stock)
    filter = 'filter_example' # str | Фильтрация отчета по ID сущностей. Поддерживаемые поля: `assortmentId`, `storeId`.  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Краткий отчет об остатках
        api_response = api_instance.get_stock_all_current(include=include, changed_since=changed_since, stock_type=stock_type, filter=filter, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsStockCurrentApi->get_stock_all_current:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsStockCurrentApi->get_stock_all_current: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **include** | **str**| Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  | [optional] 
 **changed_since** | **str**| Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: &#x60;yyyy-MM-dd HH:mm:ss&#x60;.  | [optional] 
 **stock_type** | **str**| Тип рассчитываемого значения остатка. По умолчанию &#x60;stock&#x60;.  | [optional] [default to stock]
 **filter** | **str**| Фильтрация отчета по ID сущностей. Поддерживаемые поля: &#x60;assortmentId&#x60;, &#x60;storeId&#x60;.  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**List[StockCurrentAll]**](StockCurrentAll.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_stock_by_slot_current**
> List[StockCurrentBySlot] get_stock_by_slot_current(include=include, stock_type=stock_type, filter=filter, accept=accept, accept_encoding=accept_encoding)

Получить Краткий отчет об остатках по ячейкам

Краткий отчет об остатках с группировкой по номенклатуре, складам и ячейкам.
Возвращает один тип значения остатка, выбранный параметром `stockType`.

Для запроса требуется фильтрация по `assortmentId` или `storeId`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.stock_current_by_slot import StockCurrentBySlot
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
    api_instance = moysklad_remap_12_sdk.ReportsStockCurrentApi(api_client)
    include = 'include_example' # str | Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  (optional)
    stock_type = stock # str | Тип рассчитываемого значения остатка. По умолчанию `stock`.  (optional) (default to stock)
    filter = 'filter_example' # str | Фильтрация отчета по ID сущностей. Поддерживаемые поля: `assortmentId`, `storeId`.  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Краткий отчет об остатках по ячейкам
        api_response = api_instance.get_stock_by_slot_current(include=include, stock_type=stock_type, filter=filter, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsStockCurrentApi->get_stock_by_slot_current:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsStockCurrentApi->get_stock_by_slot_current: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **include** | **str**| Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  | [optional] 
 **stock_type** | **str**| Тип рассчитываемого значения остатка. По умолчанию &#x60;stock&#x60;.  | [optional] [default to stock]
 **filter** | **str**| Фильтрация отчета по ID сущностей. Поддерживаемые поля: &#x60;assortmentId&#x60;, &#x60;storeId&#x60;.  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**List[StockCurrentBySlot]**](StockCurrentBySlot.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_stock_by_store_current**
> List[StockCurrentByStore] get_stock_by_store_current(include=include, changed_since=changed_since, stock_type=stock_type, with_recalculate=with_recalculate, filter=filter, accept=accept, accept_encoding=accept_encoding)

Получить Краткий отчет об остатках по складам

Краткий отчет об остатках с группировкой по номенклатуре и складам.
Возвращает один тип значения остатка, выбранный параметром `stockType`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.stock_current_by_store import StockCurrentByStore
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
    api_instance = moysklad_remap_12_sdk.ReportsStockCurrentApi(api_client)
    include = 'include_example' # str | Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  (optional)
    changed_since = 'changed_since_example' # str | Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: `yyyy-MM-dd HH:mm:ss`.  (optional)
    stock_type = stock # str | Тип рассчитываемого значения остатка. По умолчанию `stock`.  (optional) (default to stock)
    with_recalculate = True # bool | Включает позиции, по которым остаток пересчитывается. Для таких позиций значение остатка может быть `null`.  (optional)
    filter = 'filter_example' # str | Фильтрация отчета по ID сущностей. Поддерживаемые поля: `assortmentId`, `storeId`.  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Краткий отчет об остатках по складам
        api_response = api_instance.get_stock_by_store_current(include=include, changed_since=changed_since, stock_type=stock_type, with_recalculate=with_recalculate, filter=filter, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsStockCurrentApi->get_stock_by_store_current:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsStockCurrentApi->get_stock_by_store_current: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **include** | **str**| Управляет включением нулевых остатков. По умолчанию выводятся только ненулевые значения.  | [optional] 
 **changed_since** | **str**| Выводит фактические остатки по позициям, у которых остаток изменился с указанного момента. Формат: &#x60;yyyy-MM-dd HH:mm:ss&#x60;.  | [optional] 
 **stock_type** | **str**| Тип рассчитываемого значения остатка. По умолчанию &#x60;stock&#x60;.  | [optional] [default to stock]
 **with_recalculate** | **bool**| Включает позиции, по которым остаток пересчитывается. Для таких позиций значение остатка может быть &#x60;null&#x60;.  | [optional] 
 **filter** | **str**| Фильтрация отчета по ID сущностей. Поддерживаемые поля: &#x60;assortmentId&#x60;, &#x60;storeId&#x60;.  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**List[StockCurrentByStore]**](StockCurrentByStore.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

