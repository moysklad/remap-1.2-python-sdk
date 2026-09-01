# moysklad_remap_12_sdk.ReportsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_report_dashboard_day**](ReportsApi.md#get_report_dashboard_day) | **GET** /report/dashboard/day | Получить показатели за день
[**get_report_dashboard_month**](ReportsApi.md#get_report_dashboard_month) | **GET** /report/dashboard/month | Получить показатели за месяц
[**get_report_dashboard_week**](ReportsApi.md#get_report_dashboard_week) | **GET** /report/dashboard/week | Получить показатели за неделю
[**get_report_orders_plot_series**](ReportsApi.md#get_report_orders_plot_series) | **GET** /report/orders/plotseries | Получить показатели заказов
[**get_report_sales_plot_series**](ReportsApi.md#get_report_sales_plot_series) | **GET** /report/sales/plotseries | Получить показатели продаж


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

