# moysklad_remap_12_sdk.BonusTransactionsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_bonus_transaction**](BonusTransactionsApi.md#create_bonus_transaction) | **POST** /entity/bonustransaction | Создать бонусную операцию
[**create_bonus_transactions_batch**](BonusTransactionsApi.md#create_bonus_transactions_batch) | **POST** /entity/bonustransaction/batch | Создать или изменить бонусные операции
[**delete_bonus_transaction**](BonusTransactionsApi.md#delete_bonus_transaction) | **DELETE** /entity/bonustransaction/{id} | Удалить бонусную операцию
[**delete_bonus_transactions_batch**](BonusTransactionsApi.md#delete_bonus_transactions_batch) | **POST** /entity/bonustransaction/delete | Удалить бонусные операции
[**get_bonus_transaction_by_id**](BonusTransactionsApi.md#get_bonus_transaction_by_id) | **GET** /entity/bonustransaction/{id} | Получить бонусную операцию по ID
[**get_bonus_transactions**](BonusTransactionsApi.md#get_bonus_transactions) | **GET** /entity/bonustransaction | Получить список бонусных операций
[**update_bonus_transaction**](BonusTransactionsApi.md#update_bonus_transaction) | **PUT** /entity/bonustransaction/{id} | Изменить бонусную операцию


# **create_bonus_transaction**
> BonusTransaction create_bonus_transaction(bonus_transaction, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать бонусную операцию

Создание новой бонусной операции

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.bonus_transaction import BonusTransaction
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
    api_instance = moysklad_remap_12_sdk.BonusTransactionsApi(api_client)
    bonus_transaction = moysklad_remap_12_sdk.BonusTransaction() # BonusTransaction | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать бонусную операцию
        api_response = api_instance.create_bonus_transaction(bonus_transaction, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of BonusTransactionsApi->create_bonus_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BonusTransactionsApi->create_bonus_transaction: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bonus_transaction** | [**BonusTransaction**](BonusTransaction.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**BonusTransaction**](BonusTransaction.md)

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

# **create_bonus_transactions_batch**
> List[BatchResponseEntity] create_bonus_transactions_batch(bonus_transaction, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать или изменить бонусные операции

Создание или изменение нескольких бонусных операций.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.batch_response_entity import BatchResponseEntity
from moysklad_remap_12_sdk.models.bonus_transaction import BonusTransaction
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
    api_instance = moysklad_remap_12_sdk.BonusTransactionsApi(api_client)
    bonus_transaction = [moysklad_remap_12_sdk.BonusTransaction()] # List[BonusTransaction] | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать или изменить бонусные операции
        api_response = api_instance.create_bonus_transactions_batch(bonus_transaction, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of BonusTransactionsApi->create_bonus_transactions_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BonusTransactionsApi->create_bonus_transactions_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bonus_transaction** | [**List[BonusTransaction]**](BonusTransaction.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[BatchResponseEntity]**](BatchResponseEntity.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Бонусные операции созданы или изменены (элемент — сущность или объект ошибки) |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_bonus_transaction**
> delete_bonus_transaction(id, accept=accept, accept_encoding=accept_encoding)

Удалить бонусную операцию

Удаление бонусной операции с указанным id

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
    api_instance = moysklad_remap_12_sdk.BonusTransactionsApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить бонусную операцию
        api_instance.delete_bonus_transaction(id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling BonusTransactionsApi->delete_bonus_transaction: %s\n" % e)
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
**200** | Бонусная операция успешно удалена |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_bonus_transactions_batch**
> List[DeleteRowResult] delete_bonus_transactions_batch(bonus_transaction, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить бонусные операции

Массовое удаление бонусных операций по их мета-объектам.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.bonus_transaction import BonusTransaction
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
    api_instance = moysklad_remap_12_sdk.BonusTransactionsApi(api_client)
    bonus_transaction = [moysklad_remap_12_sdk.BonusTransaction()] # List[BonusTransaction] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить бонусные операции
        api_response = api_instance.delete_bonus_transactions_batch(bonus_transaction, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of BonusTransactionsApi->delete_bonus_transactions_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BonusTransactionsApi->delete_bonus_transactions_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bonus_transaction** | [**List[BonusTransaction]**](BonusTransaction.md)|  | 
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

# **get_bonus_transaction_by_id**
> BonusTransaction get_bonus_transaction_by_id(id, expand=expand, accept=accept, accept_encoding=accept_encoding)

Получить бонусную операцию по ID

Запрос бонусной операции с указанным id

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.bonus_transaction import BonusTransaction
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
    api_instance = moysklad_remap_12_sdk.BonusTransactionsApi(api_client)
    id = 'id_example' # str | ID сущности
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить бонусную операцию по ID
        api_response = api_instance.get_bonus_transaction_by_id(id, expand=expand, accept=accept, accept_encoding=accept_encoding)
        print("The response of BonusTransactionsApi->get_bonus_transaction_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BonusTransactionsApi->get_bonus_transaction_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**BonusTransaction**](BonusTransaction.md)

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

# **get_bonus_transactions**
> BonusTransaction get_bonus_transactions(limit=limit, offset=offset, search=search, filter=filter, expand=expand, order=order, accept=accept, accept_encoding=accept_encoding)

Получить список бонусных операций

Запрос всех бонусных операций для данной учетной записи

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.bonus_transaction import BonusTransaction
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
    api_instance = moysklad_remap_12_sdk.BonusTransactionsApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    search = 'search_example' # str | Контекстный поиск по строковым полям сущностей (optional)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    order = 'order_example' # str | Сортировка (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить список бонусных операций
        api_response = api_instance.get_bonus_transactions(limit=limit, offset=offset, search=search, filter=filter, expand=expand, order=order, accept=accept, accept_encoding=accept_encoding)
        print("The response of BonusTransactionsApi->get_bonus_transactions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BonusTransactionsApi->get_bonus_transactions: %s\n" % e)
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
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**BonusTransaction**](BonusTransaction.md)

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

# **update_bonus_transaction**
> BonusTransaction update_bonus_transaction(id, bonus_transaction, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Изменить бонусную операцию

Запрос на изменение бонусной операции с указанным id

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.bonus_transaction import BonusTransaction
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
    api_instance = moysklad_remap_12_sdk.BonusTransactionsApi(api_client)
    id = 'id_example' # str | ID сущности
    bonus_transaction = moysklad_remap_12_sdk.BonusTransaction() # BonusTransaction | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Изменить бонусную операцию
        api_response = api_instance.update_bonus_transaction(id, bonus_transaction, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of BonusTransactionsApi->update_bonus_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BonusTransactionsApi->update_bonus_transaction: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **bonus_transaction** | [**BonusTransaction**](BonusTransaction.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**BonusTransaction**](BonusTransaction.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Бонусная операция успешно обновлена |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

