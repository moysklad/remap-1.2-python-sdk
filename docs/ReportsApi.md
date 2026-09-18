# moysklad_remap_12_sdk.ReportsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_report_counterparty**](ReportsApi.md#get_report_counterparty) | **GET** /report/counterparty | Получить показатели контрагентов
[**get_report_counterparty_by_id**](ReportsApi.md#get_report_counterparty_by_id) | **GET** /report/counterparty/{id} | Получить показатели контрагента
[**get_report_dashboard_day**](ReportsApi.md#get_report_dashboard_day) | **GET** /report/dashboard/day | Получить показатели за день
[**get_report_dashboard_month**](ReportsApi.md#get_report_dashboard_month) | **GET** /report/dashboard/month | Получить показатели за месяц
[**get_report_dashboard_week**](ReportsApi.md#get_report_dashboard_week) | **GET** /report/dashboard/week | Получить показатели за неделю
[**get_report_money_by_account**](ReportsApi.md#get_report_money_by_account) | **GET** /report/money/byaccount | Получить остатки денежных средств по кассам и счетам
[**get_report_money_plot_series**](ReportsApi.md#get_report_money_plot_series) | **GET** /report/money/plotseries | Получить график движения денежных средств
[**get_report_orders_plot_series**](ReportsApi.md#get_report_orders_plot_series) | **GET** /report/orders/plotseries | Получить показатели заказов
[**get_report_profit_by_counterparty**](ReportsApi.md#get_report_profit_by_counterparty) | **GET** /report/profit/bycounterparty | Получить прибыльность по покупателям
[**get_report_profit_by_employee**](ReportsApi.md#get_report_profit_by_employee) | **GET** /report/profit/byemployee | Получить прибыльность по сотрудникам
[**get_report_profit_by_product**](ReportsApi.md#get_report_profit_by_product) | **GET** /report/profit/byproduct | Получить прибыльность по товарам
[**get_report_profit_by_sales_channel**](ReportsApi.md#get_report_profit_by_sales_channel) | **GET** /report/profit/bysaleschannel | Получить прибыльность по каналам продаж
[**get_report_profit_by_variant**](ReportsApi.md#get_report_profit_by_variant) | **GET** /report/profit/byvariant | Получить прибыльность по модификациям
[**get_report_sales_plot_series**](ReportsApi.md#get_report_sales_plot_series) | **GET** /report/sales/plotseries | Получить показатели продаж
[**get_report_turnover_all**](ReportsApi.md#get_report_turnover_all) | **GET** /report/turnover/all | Получить Обороты по товарам
[**get_report_turnover_by_operations**](ReportsApi.md#get_report_turnover_by_operations) | **GET** /report/turnover/byoperations | Получить Обороты по товару с детализацией по документам
[**get_report_turnover_by_store**](ReportsApi.md#get_report_turnover_by_store) | **GET** /report/turnover/bystore | Получить Обороты по товару с детализацией по складам
[**query_report_counterparty**](ReportsApi.md#query_report_counterparty) | **POST** /report/counterparty | Получить выборочные показатели контрагентов


# **get_report_counterparty**
> ReportCounterpartyList get_report_counterparty(limit=limit, offset=offset, filter=filter, accept=accept, accept_encoding=accept_encoding)

Получить показатели контрагентов

Запрос отчета «Показатели контрагентов» по всем контрагентам.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_counterparty_list import ReportCounterpartyList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить показатели контрагентов
        api_response = api_instance.get_report_counterparty(limit=limit, offset=offset, filter=filter, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsApi->get_report_counterparty:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_counterparty: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ReportCounterpartyList**](ReportCounterpartyList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета по контрагентам |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_counterparty_by_id**
> ReportCounterparty get_report_counterparty_by_id(id, accept=accept, accept_encoding=accept_encoding)

Получить показатели контрагента

Запрос отчета «Показатели контрагентов» по контрагенту с указанным id.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_counterparty import ReportCounterparty
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить показатели контрагента
        api_response = api_instance.get_report_counterparty_by_id(id, accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsApi->get_report_counterparty_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_counterparty_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ReportCounterparty**](ReportCounterparty.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета по контрагенту |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_dashboard_day**
> ReportDashboard get_report_dashboard_day(accept=accept, accept_encoding=accept_encoding)

Получить показатели за день

Запрос показателей за день.
Для доступа к отчету требуется право на просмотр показателей `viewDashboard`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_dashboard import ReportDashboard
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить показатели за день
        api_response = api_instance.get_report_dashboard_day(accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsApi->get_report_dashboard_day:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_dashboard_day: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ReportDashboard**](ReportDashboard.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. JSON представление показателей за день |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_dashboard_month**
> ReportDashboard get_report_dashboard_month(accept=accept, accept_encoding=accept_encoding)

Получить показатели за месяц

Запрос показателей за месяц.
Для доступа к отчету требуется право на просмотр показателей `viewDashboard`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_dashboard import ReportDashboard
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить показатели за месяц
        api_response = api_instance.get_report_dashboard_month(accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsApi->get_report_dashboard_month:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_dashboard_month: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ReportDashboard**](ReportDashboard.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. JSON представление показателей за месяц |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_dashboard_week**
> ReportDashboard get_report_dashboard_week(accept=accept, accept_encoding=accept_encoding)

Получить показатели за неделю

Запрос показателей за неделю.
Для доступа к отчету требуется право на просмотр показателей `viewDashboard`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_dashboard import ReportDashboard
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить показатели за неделю
        api_response = api_instance.get_report_dashboard_week(accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsApi->get_report_dashboard_week:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_dashboard_week: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ReportDashboard**](ReportDashboard.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. JSON представление показателей за неделю |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_money_by_account**
> ReportMoneyByAccountList get_report_money_by_account(accept=accept, accept_encoding=accept_encoding)

Получить остатки денежных средств по кассам и счетам

Запрос текущих остатков денежных средств по кассам и счетам организаций.
Для доступа к отчету требуется право на просмотр показателей `viewDashboard`
и право «Видеть остатки денег» `viewMoneyDashboard`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_money_by_account_list import ReportMoneyByAccountList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить остатки денежных средств по кассам и счетам
        api_response = api_instance.get_report_money_by_account(accept=accept, accept_encoding=accept_encoding)
        print("The response of ReportsApi->get_report_money_by_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_money_by_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**ReportMoneyByAccountList**](ReportMoneyByAccountList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. JSON представление отчета об остатках денежных средств |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_money_plot_series**
> ReportMoneyPlotSeries get_report_money_plot_series(moment_from, moment_to, interval, filter=filter, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить график движения денежных средств

Запрос отчета о движении денежных средств за период с разбивкой по часам, дням или месяцам.
Для доступа к отчету требуется право на просмотр показателей `viewDashboard`
и право «Видеть остатки денег» `viewMoneyDashboard`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_money_plot_series import ReportMoneyPlotSeries
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
    interval = 'interval_example' # str | Интервал построения отчета
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить график движения денежных средств
        api_response = api_instance.get_report_money_plot_series(moment_from, moment_to, interval, filter=filter, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_money_plot_series:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_money_plot_series: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | 
 **interval** | **str**| Интервал построения отчета | 
 **filter** | **str**| Фильтрация выборки | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportMoneyPlotSeries**](ReportMoneyPlotSeries.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. JSON представление отчета о движении денежных средств |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_orders_plot_series**
> ReportOrdersPlotSeriesList get_report_orders_plot_series(moment_from, moment_to, interval, filter=filter, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить показатели заказов

Запрос показателей заказов покупателей за период с разбивкой по часам, дням или месяцам.
Для доступа к отчету требуется право на просмотр показателей `viewDashboard`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_orders_plot_series_list import ReportOrdersPlotSeriesList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
    interval = 'interval_example' # str | Интервал построения отчета
    filter = 'filter_example' # str | Фильтрация показателей заказов. Доступные поля: `organization`, `store`, `project`. Можно указать несколько значений; пустые значения недопустимы.  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить показатели заказов
        api_response = api_instance.get_report_orders_plot_series(moment_from, moment_to, interval, filter=filter, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_orders_plot_series:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_orders_plot_series: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | 
 **interval** | **str**| Интервал построения отчета | 
 **filter** | **str**| Фильтрация показателей заказов. Доступные поля: &#x60;organization&#x60;, &#x60;store&#x60;, &#x60;project&#x60;. Можно указать несколько значений; пустые значения недопустимы.  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportOrdersPlotSeriesList**](ReportOrdersPlotSeriesList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. JSON представление отчета показателей заказов |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_profit_by_counterparty**
> ReportProfitByCounterpartyList get_report_profit_by_counterparty(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить прибыльность по покупателям

Запрос отчета «Прибыльность по покупателям».
Для доступа к отчету требуется право на просмотр отчета «Прибыльность».


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_profit_by_counterparty_list import ReportProfitByCounterpartyList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить прибыльность по покупателям
        api_response = api_instance.get_report_profit_by_counterparty(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_profit_by_counterparty:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_profit_by_counterparty: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportProfitByCounterpartyList**](ReportProfitByCounterpartyList.md)

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

# **get_report_profit_by_employee**
> ReportProfitByEmployeeList get_report_profit_by_employee(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить прибыльность по сотрудникам

Запрос отчета «Прибыльность по сотрудникам».
Для доступа к отчету требуется право на просмотр отчета «Прибыльность».


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_profit_by_employee_list import ReportProfitByEmployeeList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить прибыльность по сотрудникам
        api_response = api_instance.get_report_profit_by_employee(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_profit_by_employee:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_profit_by_employee: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportProfitByEmployeeList**](ReportProfitByEmployeeList.md)

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

# **get_report_profit_by_product**
> ReportProfitByProductList get_report_profit_by_product(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить прибыльность по товарам

Запрос отчета «Прибыльность по товарам». В отчете учитываются товары, услуги и комплекты.
Для доступа к отчету требуется право на просмотр отчета «Прибыльность».


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_profit_by_product_list import ReportProfitByProductList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить прибыльность по товарам
        api_response = api_instance.get_report_profit_by_product(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_profit_by_product:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_profit_by_product: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportProfitByProductList**](ReportProfitByProductList.md)

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

# **get_report_profit_by_sales_channel**
> ReportProfitBySalesChannelList get_report_profit_by_sales_channel(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить прибыльность по каналам продаж

Запрос отчета «Прибыльность по каналам продаж».
Для доступа к отчету требуется право на просмотр отчета «Прибыльность».


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_profit_by_sales_channel_list import ReportProfitBySalesChannelList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить прибыльность по каналам продаж
        api_response = api_instance.get_report_profit_by_sales_channel(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_profit_by_sales_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_profit_by_sales_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportProfitBySalesChannelList**](ReportProfitBySalesChannelList.md)

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

# **get_report_profit_by_variant**
> ReportProfitByVariantList get_report_profit_by_variant(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить прибыльность по модификациям

Запрос отчета «Прибыльность по модификациям». В отчете учитываются модификации,
товары, услуги и комплекты.
Для доступа к отчету требуется право на просмотр отчета «Прибыльность».


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_profit_by_variant_list import ReportProfitByVariantList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить прибыльность по модификациям
        api_response = api_instance.get_report_profit_by_variant(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_profit_by_variant:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_profit_by_variant: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportProfitByVariantList**](ReportProfitByVariantList.md)

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

# **get_report_sales_plot_series**
> ReportSalesPlotSeriesList get_report_sales_plot_series(moment_from, moment_to, interval, filter=filter, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить показатели продаж

Запрос показателей продаж за период с разбивкой по часам, дням или месяцам.
В показателях продаж учитываются отгрузки, розничные продажи и полученные отчеты комиссионера.
Для доступа к отчету требуется право на просмотр показателей `viewDashboard`.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_sales_plot_series_list import ReportSalesPlotSeriesList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS
    interval = 'interval_example' # str | Интервал построения отчета
    filter = 'filter_example' # str | Фильтрация показателей продаж. Доступные поля: `organization`, `store`, `project`, `retailStore`. Можно указать несколько значений; пустые значения недопустимы.  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить показатели продаж
        api_response = api_instance.get_report_sales_plot_series(moment_from, moment_to, interval, filter=filter, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_sales_plot_series:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_sales_plot_series: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | 
 **interval** | **str**| Интервал построения отчета | 
 **filter** | **str**| Фильтрация показателей продаж. Доступные поля: &#x60;organization&#x60;, &#x60;store&#x60;, &#x60;project&#x60;, &#x60;retailStore&#x60;. Можно указать несколько значений; пустые значения недопустимы.  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportSalesPlotSeriesList**](ReportSalesPlotSeriesList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. JSON представление отчета показателей продаж |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_turnover_all**
> ReportTurnoverList get_report_turnover_all(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, group_by=group_by, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить Обороты по товарам

Запрос отчета «Обороты по товарам» — общий отчет по оборотам товаров и модификаций.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_turnover_list import ReportTurnoverList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    group_by = product # str | Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию `product`. (optional) (default to product)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить Обороты по товарам
        api_response = api_instance.get_report_turnover_all(limit=limit, offset=offset, filter=filter, moment_from=moment_from, moment_to=moment_to, group_by=group_by, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_turnover_all:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_turnover_all: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **group_by** | **str**| Тип, по которому нужно сгруппировать выдачу. Значение по умолчанию &#x60;product&#x60;. | [optional] [default to product]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportTurnoverList**](ReportTurnoverList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_turnover_by_operations**
> ReportTurnoverByOperationList get_report_turnover_by_operations(filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить Обороты по товару с детализацией по документам

Запрос отчета «Обороты по товару с детализацией по документам».

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_turnover_by_operation_list import ReportTurnoverByOperationList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить Обороты по товару с детализацией по документам
        api_response = api_instance.get_report_turnover_by_operations(filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_turnover_by_operations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_turnover_by_operations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportTurnoverByOperationList**](ReportTurnoverByOperationList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_report_turnover_by_store**
> ReportTurnoverByStoreList get_report_turnover_by_store(filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)

Получить Обороты по товару с детализацией по складам

Запрос отчета «Обороты по товару с детализацией по складам».

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_turnover_by_store_list import ReportTurnoverByStoreList
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    moment_from = 'moment_from_example' # str | Начало периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    moment_to = 'moment_to_example' # str | Конец периода отчета в формате YYYY-MM-DD HH:MM:SS (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    x_lognex_accept_timezone = 'x_lognex_accept_timezone_example' # str | Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: `Wed, 16 Aug 2017 23:07:01 +0700`. При подсчете показателей даты операций смещаются в таймзону клиента.  (optional)

    try:
        # Получить Обороты по товару с детализацией по складам
        api_response = api_instance.get_report_turnover_by_store(filter=filter, moment_from=moment_from, moment_to=moment_to, accept=accept, accept_encoding=accept_encoding, x_lognex_accept_timezone=x_lognex_accept_timezone)
        print("The response of ReportsApi->get_report_turnover_by_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->get_report_turnover_by_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **str**| Фильтрация выборки | [optional] 
 **moment_from** | **str**| Начало периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **moment_to** | **str**| Конец периода отчета в формате YYYY-MM-DD HH:MM:SS | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **x_lognex_accept_timezone** | **str**| Опциональный заголовок, в котором указана текущая дата на клиенте в RFC 3522. Таймзону обязательно указывать в формате знак и 4 символа. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;. При подсчете показателей даты операций смещаются в таймзону клиента.  | [optional] 

### Return type

[**ReportTurnoverByStoreList**](ReportTurnoverByStoreList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета |  * X-Lognex-Content-Timezone - Заголовок ответа. В нем указывается (как думает сервер) текущая дата на клиенте в RFC 3522. Пример: &#x60;Wed, 16 Aug 2017 23:07:01 +0700&#x60;.  <br>  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **query_report_counterparty**
> ReportCounterpartyList query_report_counterparty(report_counterparty_query, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Получить выборочные показатели контрагентов

Запрос отчета «Показатели контрагентов» по указанным контрагентам.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.report_counterparty_list import ReportCounterpartyList
from moysklad_remap_12_sdk.models.report_counterparty_query import ReportCounterpartyQuery
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
    api_instance = moysklad_remap_12_sdk.ReportsApi(api_client)
    report_counterparty_query = moysklad_remap_12_sdk.ReportCounterpartyQuery() # ReportCounterpartyQuery | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Получить выборочные показатели контрагентов
        api_response = api_instance.query_report_counterparty(report_counterparty_query, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of ReportsApi->query_report_counterparty:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->query_report_counterparty: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **report_counterparty_query** | [**ReportCounterpartyQuery**](ReportCounterpartyQuery.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**ReportCounterpartyList**](ReportCounterpartyList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление отчета по указанным контрагентам |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

