# moysklad_remap_12_sdk.ReportsStockByOperationApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_stock_by_operation**](ReportsStockByOperationApi.md#get_stock_by_operation) | **GET** /report/stock/byoperation | Получить Остатки по документу


# **get_stock_by_operation**
> StockByOperationList get_stock_by_operation(operation_id, accept=accept, accept_encoding=accept_encoding)

Получить Остатки по документу

Запрос отчета «Остатки по документам» — остатки по позициям указанного документа
со склада документа, а также себестоимость позиций по FIFO с учётом количества.

Обязательный параметр — `operation.id` (ID документа).

Поддерживаемые типы документов: отгрузка, заказ покупателя, розничная продажа,
счет поставщика, счет покупателю, заказ поставщику, приемка, розничный возврат,
возврат поставщику, возврат покупателя.

Для отгрузки, розничной продажи, приемки, возвратов остатки рассчитываются на момент
поля `moment` документа. Для заказа покупателя, счетов и заказа поставщику —
на текущий момент времени.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.stock_by_operation_list import StockByOperationList
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
    api_instance = moysklad_remap_12_sdk.ReportsStockByOperationApi(api_client)
    operation_id = 'operation_id_example' # str | ID документа, по которому нужно получить остатки
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Остатки по документу
        api_response = api_instance.get_stock_by_operation(operation_id, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsStockByOperationApi->get_stock_by_operation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsStockByOperationApi->get_stock_by_operation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **operation_id** | **str**| ID документа, по которому нужно получить остатки | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**StockByOperationList**](StockByOperationList.md)

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

