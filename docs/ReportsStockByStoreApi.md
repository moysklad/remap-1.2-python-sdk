# moysklad_remap_12_sdk.ReportsStockByStoreApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_stock_by_store**](ReportsStockByStoreApi.md#get_stock_by_store) | **GET** /report/stock/bystore | Получить Остатки по складам


# **get_stock_by_store**
> StockByStoreList get_stock_by_store(limit=limit, offset=offset, filter=filter, order=order, group_by=group_by, accept=accept, accept_encoding=accept_encoding)

Получить Остатки по складам

Запрос отчета «Остатки по складам» — остаток по каждому товару на каждом складе.
Тип объектов в выдаче задается параметром `groupBy`: товары (product), товары и модификации
(variant), товары, модификации и партии (consignment).


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.stock_by_store_list import StockByStoreList
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
    api_instance = moysklad_remap_12_sdk.ReportsStockByStoreApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    order = 'order_example' # str | Сортировка (optional)
    group_by = 'group_by_example' # str | Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию `variant`. - `product` — выдает только товары - `variant` — выдает товары и модификации - `consignment` — выдает товары, модификации, партии  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Остатки по складам
        api_response = api_instance.get_stock_by_store(limit=limit, offset=offset, filter=filter, order=order, group_by=group_by, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsStockByStoreApi->get_stock_by_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsStockByStoreApi->get_stock_by_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **order** | **str**| Сортировка | [optional] 
 **group_by** | **str**| Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию &#x60;variant&#x60;. - &#x60;product&#x60; — выдает только товары - &#x60;variant&#x60; — выдает товары и модификации - &#x60;consignment&#x60; — выдает товары, модификации, партии  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**StockByStoreList**](StockByStoreList.md)

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

