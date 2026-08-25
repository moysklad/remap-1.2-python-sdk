# moysklad_remap_12_sdk.CustomerOrdersApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_customer_order**](CustomerOrdersApi.md#create_customer_order) | **POST** /entity/customerorder | Создать CustomerOrders
[**create_customer_order_batch**](CustomerOrdersApi.md#create_customer_order_batch) | **POST** /entity/customerorder/batch | Массовое создание и обновление CustomerOrders
[**create_customer_order_metadata_attribute**](CustomerOrdersApi.md#create_customer_order_metadata_attribute) | **POST** /entity/customerorder/metadata/attributes | Создать Доп. поле CustomerOrder
[**create_customer_order_metadata_state**](CustomerOrdersApi.md#create_customer_order_metadata_state) | **POST** /entity/customerorder/metadata/states | Создать статус CustomerOrder
[**create_customer_order_metadata_states_batch**](CustomerOrdersApi.md#create_customer_order_metadata_states_batch) | **POST** /entity/customerorder/metadata/states/batch | Массовое создание и обновление статусов CustomerOrder
[**create_customer_order_note**](CustomerOrdersApi.md#create_customer_order_note) | **POST** /entity/customerorder/{id}/notes | Добавить Событие Заказа покупателя
[**create_customer_order_position**](CustomerOrdersApi.md#create_customer_order_position) | **POST** /entity/customerorder/{id}/positions | Создать и обновить позицию Заказа покупателя
[**create_customer_order_positions**](CustomerOrdersApi.md#create_customer_order_positions) | **POST** /entity/customerorder/{id}/positions/batch | Массовое создание и обновление позиций Заказа покупателя
[**create_customer_order_publication**](CustomerOrdersApi.md#create_customer_order_publication) | **POST** /entity/customerorder/{id}/publication | Создать Публикацию Заказа покупателя
[**delete_customer_order**](CustomerOrdersApi.md#delete_customer_order) | **DELETE** /entity/customerorder/{id} | Удалить CustomerOrders
[**delete_customer_order_batch**](CustomerOrdersApi.md#delete_customer_order_batch) | **POST** /entity/customerorder/delete | Массовое удаление CustomerOrders
[**delete_customer_order_metadata_attribute_by_id**](CustomerOrdersApi.md#delete_customer_order_metadata_attribute_by_id) | **DELETE** /entity/customerorder/metadata/attributes/{id} | Удалить отдельное доп. поле CustomerOrder
[**delete_customer_order_metadata_state_by_id**](CustomerOrdersApi.md#delete_customer_order_metadata_state_by_id) | **DELETE** /entity/customerorder/metadata/states/{id} | Удалить отдельный статус CustomerOrder
[**delete_customer_order_note**](CustomerOrdersApi.md#delete_customer_order_note) | **DELETE** /entity/customerorder/{id}/notes/{noteId} | Удалить Событие Заказа покупателя
[**delete_customer_order_position**](CustomerOrdersApi.md#delete_customer_order_position) | **DELETE** /entity/customerorder/{id}/positions/{positionId} | Удалить позицию CustomerOrders
[**delete_customer_order_positions_batch**](CustomerOrdersApi.md#delete_customer_order_positions_batch) | **POST** /entity/customerorder/{id}/positions/delete | Массовое удаление позиций CustomerOrders
[**delete_customer_order_publication**](CustomerOrdersApi.md#delete_customer_order_publication) | **DELETE** /entity/customerorder/{id}/publication/{publicationId} | Удалить Публикацию Заказа покупателя
[**export_customer_order**](CustomerOrdersApi.md#export_customer_order) | **POST** /entity/customerorder/{id}/export | Запрос на печать Заказа покупателя
[**get_customer_order_audit_events**](CustomerOrdersApi.md#get_customer_order_audit_events) | **GET** /entity/customerorder/{id}/audit | Получить события аудита Заказа покупателя
[**get_customer_order_by_id**](CustomerOrdersApi.md#get_customer_order_by_id) | **GET** /entity/customerorder/{id} | Получить CustomerOrders
[**get_customer_order_list**](CustomerOrdersApi.md#get_customer_order_list) | **GET** /entity/customerorder | Получить список CustomerOrders
[**get_customer_order_metadata**](CustomerOrdersApi.md#get_customer_order_metadata) | **GET** /entity/customerorder/metadata | Метаданные CustomerOrders
[**get_customer_order_metadata_attribute**](CustomerOrdersApi.md#get_customer_order_metadata_attribute) | **GET** /entity/customerorder/metadata/attributes | Доп. поля CustomerOrder
[**get_customer_order_metadata_attribute_by_id**](CustomerOrdersApi.md#get_customer_order_metadata_attribute_by_id) | **GET** /entity/customerorder/metadata/attributes/{id} | Отдельное доп. поле CustomerOrder
[**get_customer_order_metadata_state_by_id**](CustomerOrdersApi.md#get_customer_order_metadata_state_by_id) | **GET** /entity/customerorder/metadata/states/{id} | Отдельный статус CustomerOrder
[**get_customer_order_note_by_id**](CustomerOrdersApi.md#get_customer_order_note_by_id) | **GET** /entity/customerorder/{id}/notes/{noteId} | Получить Событие Заказа покупателя по ID
[**get_customer_order_notes**](CustomerOrdersApi.md#get_customer_order_notes) | **GET** /entity/customerorder/{id}/notes | Получить список Событий Заказа покупателя
[**get_customer_order_position_by_id**](CustomerOrdersApi.md#get_customer_order_position_by_id) | **GET** /entity/customerorder/{id}/positions/{positionId} | Получить позицию CustomerOrders
[**get_customer_order_positions**](CustomerOrdersApi.md#get_customer_order_positions) | **GET** /entity/customerorder/{id}/positions | Получить позиции CustomerOrders
[**get_customer_order_publication_by_id**](CustomerOrdersApi.md#get_customer_order_publication_by_id) | **GET** /entity/customerorder/{id}/publication/{publicationId} | Получить Публикацию Заказа покупателя
[**get_customer_order_publications**](CustomerOrdersApi.md#get_customer_order_publications) | **GET** /entity/customerorder/{id}/publication | Получить список Публикаций Заказа покупателя
[**get_customer_order_template**](CustomerOrdersApi.md#get_customer_order_template) | **PUT** /entity/customerorder/new | Шаблон CustomerOrders
[**update_customer_order**](CustomerOrdersApi.md#update_customer_order) | **PUT** /entity/customerorder/{id} | Изменить CustomerOrders
[**update_customer_order_metadata_attribute_by_id**](CustomerOrdersApi.md#update_customer_order_metadata_attribute_by_id) | **PUT** /entity/customerorder/metadata/attributes/{id} | Обновить отдельное доп. поле CustomerOrder
[**update_customer_order_metadata_state_by_id**](CustomerOrdersApi.md#update_customer_order_metadata_state_by_id) | **PUT** /entity/customerorder/metadata/states/{id} | Обновить отдельный статус CustomerOrder
[**update_customer_order_note**](CustomerOrdersApi.md#update_customer_order_note) | **PUT** /entity/customerorder/{id}/notes/{noteId} | Обновить Событие Заказа покупателя
[**update_customer_order_position**](CustomerOrdersApi.md#update_customer_order_position) | **PUT** /entity/customerorder/{id}/positions/{positionId} | Изменить позицию CustomerOrders


# **create_customer_order**
> CustomerOrder create_customer_order(customer_order, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order import CustomerOrder
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    customer_order = moysklad_remap_12_sdk.CustomerOrder() # CustomerOrder | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать CustomerOrders
        api_response = api_instance.create_customer_order(customer_order, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_order** | [**CustomerOrder**](CustomerOrder.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**CustomerOrder**](CustomerOrder.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_batch**
> List[BatchResponseEntity] create_customer_order_batch(customer_order, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое создание и обновление CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.batch_response_entity import BatchResponseEntity
from moysklad_remap_12_sdk.models.customer_order import CustomerOrder
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    customer_order = [moysklad_remap_12_sdk.CustomerOrder()] # List[CustomerOrder] | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое создание и обновление CustomerOrders
        api_response = api_instance.create_customer_order_batch(customer_order, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_order** | [**List[CustomerOrder]**](CustomerOrder.md)|  | 
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
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_metadata_attribute**
> AttributeMetaInfo create_customer_order_metadata_attribute(attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать Доп. поле CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    attribute_meta_info = moysklad_remap_12_sdk.AttributeMetaInfo() # AttributeMetaInfo | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать Доп. поле CustomerOrder
        api_response = api_instance.create_customer_order_metadata_attribute(attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_metadata_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_metadata_attribute: %s\n" % e)
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_metadata_state**
> State create_customer_order_metadata_state(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать статус CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    state = moysklad_remap_12_sdk.State() # State | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать статус CustomerOrder
        api_response = api_instance.create_customer_order_metadata_state(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_metadata_state:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_metadata_state: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_metadata_states_batch**
> List[StateRowResult] create_customer_order_metadata_states_batch(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое создание и обновление статусов CustomerOrder

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.state import State
from moysklad_remap_12_sdk.models.state_row_result import StateRowResult
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    state = [moysklad_remap_12_sdk.State()] # List[State] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое создание и обновление статусов CustomerOrder
        api_response = api_instance.create_customer_order_metadata_states_batch(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_metadata_states_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_metadata_states_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **state** | [**List[State]**](State.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[StateRowResult]**](StateRowResult.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_note**
> List[EventNote] create_customer_order_note(id, event_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Добавить Событие Заказа покупателя

Запрос на добавление одного События Заказа покупателя

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.event_note import EventNote
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    event_note = moysklad_remap_12_sdk.EventNote() # EventNote | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Добавить Событие Заказа покупателя
        api_response = api_instance.create_customer_order_note(id, event_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_note:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **event_note** | [**EventNote**](EventNote.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[EventNote]**](EventNote.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Событие успешно создано |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_position**
> List[CustomerOrderPosition] create_customer_order_position(id, customer_order_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать и обновить позицию Заказа покупателя

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order_position import CustomerOrderPosition
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    customer_order_position = moysklad_remap_12_sdk.CustomerOrderPosition() # CustomerOrderPosition | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать и обновить позицию Заказа покупателя
        api_response = api_instance.create_customer_order_position(id, customer_order_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_position:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_position: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **customer_order_position** | [**CustomerOrderPosition**](CustomerOrderPosition.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[CustomerOrderPosition]**](CustomerOrderPosition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_positions**
> List[CreateCustomerOrderPositions200ResponseInner] create_customer_order_positions(id, customer_order_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое создание и обновление позиций Заказа покупателя

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.create_customer_order_positions200_response_inner import CreateCustomerOrderPositions200ResponseInner
from moysklad_remap_12_sdk.models.customer_order_position import CustomerOrderPosition
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    customer_order_position = [moysklad_remap_12_sdk.CustomerOrderPosition()] # List[CustomerOrderPosition] | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое создание и обновление позиций Заказа покупателя
        api_response = api_instance.create_customer_order_positions(id, customer_order_position, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_positions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_positions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **customer_order_position** | [**List[CustomerOrderPosition]**](CustomerOrderPosition.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[CreateCustomerOrderPositions200ResponseInner]**](CreateCustomerOrderPositions200ResponseInner.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_customer_order_publication**
> Publication create_customer_order_publication(id, publication, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать Публикацию Заказа покупателя

Запрос на публикацию Заказа покупателя.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.publication import Publication
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    publication = moysklad_remap_12_sdk.Publication() # Publication | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать Публикацию Заказа покупателя
        api_response = api_instance.create_customer_order_publication(id, publication, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->create_customer_order_publication:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->create_customer_order_publication: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **publication** | [**Publication**](Publication.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**Publication**](Publication.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**201** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order**
> delete_customer_order(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить CustomerOrders

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить CustomerOrders
        api_instance.delete_customer_order(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order_batch**
> List[DeleteRowResult] delete_customer_order_batch(customer_order, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое удаление CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order import CustomerOrder
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    customer_order = [moysklad_remap_12_sdk.CustomerOrder()] # List[CustomerOrder] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое удаление CustomerOrders
        api_response = api_instance.delete_customer_order_batch(customer_order, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->delete_customer_order_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_order** | [**List[CustomerOrder]**](CustomerOrder.md)|  | 
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order_metadata_attribute_by_id**
> delete_customer_order_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить отдельное доп. поле CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить отдельное доп. поле CustomerOrder
        api_instance.delete_customer_order_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order_metadata_attribute_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order_metadata_state_by_id**
> delete_customer_order_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить отдельный статус CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить отдельный статус CustomerOrder
        api_instance.delete_customer_order_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order_metadata_state_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order_note**
> delete_customer_order_note(id, note_id, accept=accept, accept_encoding=accept_encoding)

Удалить Событие Заказа покупателя

Запрос на удаление одного События Заказа покупателя

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    note_id = 'note_id_example' # str | ID События
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить Событие Заказа покупателя
        api_instance.delete_customer_order_note(id, note_id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **note_id** | **str**| ID События | 
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
**204** | Событие успешно удалено |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order_position**
> delete_customer_order_position(id, position_id, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить позицию CustomerOrders

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    position_id = 'position_id_example' # str | ID позиции
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить позицию CustomerOrders
        api_instance.delete_customer_order_position(id, position_id, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order_position: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **position_id** | **str**| ID позиции | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order_positions_batch**
> List[DeleteRowResult] delete_customer_order_positions_batch(id, customer_order_position, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое удаление позиций CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order_position import CustomerOrderPosition
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    customer_order_position = [moysklad_remap_12_sdk.CustomerOrderPosition()] # List[CustomerOrderPosition] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое удаление позиций CustomerOrders
        api_response = api_instance.delete_customer_order_positions_batch(id, customer_order_position, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->delete_customer_order_positions_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order_positions_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **customer_order_position** | [**List[CustomerOrderPosition]**](CustomerOrderPosition.md)|  | 
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_customer_order_publication**
> delete_customer_order_publication(id, publication_id, accept=accept, accept_encoding=accept_encoding)

Удалить Публикацию Заказа покупателя

Запрос на удаление Публикации Заказа покупателя по идентификатору.

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    publication_id = 'publication_id_example' # str | ID публикации
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить Публикацию Заказа покупателя
        api_instance.delete_customer_order_publication(id, publication_id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->delete_customer_order_publication: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **publication_id** | **str**| ID публикации | 
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
**204** | Публикация успешно удалена |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_customer_order**
> export_customer_order(id, export_request, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Запрос на печать Заказа покупателя

Запрос на формирование печатной формы для Заказа покупателя.
При готовности сервер возвращает пустой ответ с кодом 303 и заголовком Location.


### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.export_request import ExportRequest
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    export_request = moysklad_remap_12_sdk.ExportRequest() # ExportRequest | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Запрос на печать Заказа покупателя
        api_instance.export_customer_order(id, export_request, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->export_customer_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **export_request** | [**ExportRequest**](ExportRequest.md)|  | 
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_audit_events**
> Dict[str, object] get_customer_order_audit_events(id, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)

Получить события аудита Заказа покупателя

Возвращает список событий аудита для Заказа покупателя по его ID.


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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить события аудита Заказа покупателя
        api_response = api_instance.get_customer_order_audit_events(id, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)
        print("The response of CustomerOrdersApi->get_customer_order_audit_events:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_audit_events: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

**Dict[str, object]**

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_by_id**
> CustomerOrder get_customer_order_by_id(id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)

Получить CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order import CustomerOrder
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить CustomerOrders
        api_response = api_instance.get_customer_order_by_id(id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)
        print("The response of CustomerOrdersApi->get_customer_order_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_by_id: %s\n" % e)
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

[**CustomerOrder**](CustomerOrder.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_list**
> CustomerOrderList get_customer_order_list(limit=limit, offset=offset, search=search, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Получить список CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order_list import CustomerOrderList
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    search = 'search_example' # str | Контекстный поиск по строковым полям сущностей (optional)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Получить список CustomerOrders
        api_response = api_instance.get_customer_order_list(limit=limit, offset=offset, search=search, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->get_customer_order_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_list: %s\n" % e)
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
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**CustomerOrderList**](CustomerOrderList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_metadata**
> DocumentMetadata get_customer_order_metadata(accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Метаданные CustomerOrders

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Метаданные CustomerOrders
        api_response = api_instance.get_customer_order_metadata(accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->get_customer_order_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_metadata: %s\n" % e)
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_metadata_attribute**
> AttributeMetaInfoList get_customer_order_metadata_attribute(offset=offset, limit=limit, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Доп. поля CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Доп. поля CustomerOrder
        api_response = api_instance.get_customer_order_metadata_attribute(offset=offset, limit=limit, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->get_customer_order_metadata_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_metadata_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_metadata_attribute_by_id**
> AttributeMetaInfo get_customer_order_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Отдельное доп. поле CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Отдельное доп. поле CustomerOrder
        api_response = api_instance.get_customer_order_metadata_attribute_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->get_customer_order_metadata_attribute_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_metadata_attribute_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_metadata_state_by_id**
> State get_customer_order_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Отдельный статус CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Отдельный статус CustomerOrder
        api_response = api_instance.get_customer_order_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->get_customer_order_metadata_state_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_metadata_state_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_note_by_id**
> EventNote get_customer_order_note_by_id(id, note_id, accept=accept, accept_encoding=accept_encoding)

Получить Событие Заказа покупателя по ID

Запрос на получение одного События Заказа покупателя

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.event_note import EventNote
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    note_id = 'note_id_example' # str | ID События
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Событие Заказа покупателя по ID
        api_response = api_instance.get_customer_order_note_by_id(id, note_id, accept=accept, accept_encoding=accept_encoding)
        print("The response of CustomerOrdersApi->get_customer_order_note_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_note_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **note_id** | **str**| ID События | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**EventNote**](EventNote.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_notes**
> EventNoteList get_customer_order_notes(id, limit=limit, offset=offset, expand=expand, accept=accept, accept_encoding=accept_encoding)

Получить список Событий Заказа покупателя

Запрос на получение всех Событий Заказа покупателя для данной учетной записи

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.event_note_list import EventNoteList
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить список Событий Заказа покупателя
        api_response = api_instance.get_customer_order_notes(id, limit=limit, offset=offset, expand=expand, accept=accept, accept_encoding=accept_encoding)
        print("The response of CustomerOrdersApi->get_customer_order_notes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_notes: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**EventNoteList**](EventNoteList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_position_by_id**
> CustomerOrderPosition get_customer_order_position_by_id(id, position_id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Получить позицию CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order_position import CustomerOrderPosition
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    position_id = 'position_id_example' # str | ID позиции
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Получить позицию CustomerOrders
        api_response = api_instance.get_customer_order_position_by_id(id, position_id, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->get_customer_order_position_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_position_by_id: %s\n" % e)
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
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**CustomerOrderPosition**](CustomerOrderPosition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_positions**
> CustomerOrderPositionList get_customer_order_positions(id, limit=limit, offset=offset, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)

Получить позиции CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order_position_list import CustomerOrderPositionList
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить позиции CustomerOrders
        api_response = api_instance.get_customer_order_positions(id, limit=limit, offset=offset, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding)
        print("The response of CustomerOrdersApi->get_customer_order_positions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_positions: %s\n" % e)
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

[**CustomerOrderPositionList**](CustomerOrderPositionList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_publication_by_id**
> Publication get_customer_order_publication_by_id(id, publication_id, accept=accept, accept_encoding=accept_encoding)

Получить Публикацию Заказа покупателя

Запрос на получение Публикации Заказа покупателя по идентификатору.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.publication import Publication
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    publication_id = 'publication_id_example' # str | ID публикации
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Публикацию Заказа покупателя
        api_response = api_instance.get_customer_order_publication_by_id(id, publication_id, accept=accept, accept_encoding=accept_encoding)
        print("The response of CustomerOrdersApi->get_customer_order_publication_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_publication_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **publication_id** | **str**| ID публикации | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**Publication**](Publication.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_publications**
> PublicationList get_customer_order_publications(id, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)

Получить список Публикаций Заказа покупателя

Запрос на получение списка Публикаций по указанному Заказу покупателя.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.publication_list import PublicationList
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить список Публикаций Заказа покупателя
        api_response = api_instance.get_customer_order_publications(id, limit=limit, offset=offset, accept=accept, accept_encoding=accept_encoding)
        print("The response of CustomerOrdersApi->get_customer_order_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**PublicationList**](PublicationList.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_customer_order_template**
> CustomerOrder get_customer_order_template(accept=accept, accept_encoding=accept_encoding, content_type=content_type, body=body)

Шаблон CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order import CustomerOrder
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)
    body = None # object |  (optional)

    try:
        # Шаблон CustomerOrders
        api_response = api_instance.get_customer_order_template(accept=accept, accept_encoding=accept_encoding, content_type=content_type, body=body)
        print("The response of CustomerOrdersApi->get_customer_order_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->get_customer_order_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]
 **body** | **object**|  | [optional] 

### Return type

[**CustomerOrder**](CustomerOrder.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_customer_order**
> CustomerOrder update_customer_order(id, customer_order, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Изменить CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order import CustomerOrder
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    customer_order = moysklad_remap_12_sdk.CustomerOrder() # CustomerOrder | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Изменить CustomerOrders
        api_response = api_instance.update_customer_order(id, customer_order, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->update_customer_order:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->update_customer_order: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **customer_order** | [**CustomerOrder**](CustomerOrder.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**CustomerOrder**](CustomerOrder.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_customer_order_metadata_attribute_by_id**
> AttributeMetaInfo update_customer_order_metadata_attribute_by_id(id, attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить отдельное доп. поле CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    attribute_meta_info = moysklad_remap_12_sdk.AttributeMetaInfo() # AttributeMetaInfo | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить отдельное доп. поле CustomerOrder
        api_response = api_instance.update_customer_order_metadata_attribute_by_id(id, attribute_meta_info, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->update_customer_order_metadata_attribute_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->update_customer_order_metadata_attribute_by_id: %s\n" % e)
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_customer_order_metadata_state_by_id**
> State update_customer_order_metadata_state_by_id(id, state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить отдельный статус CustomerOrder

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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    state = moysklad_remap_12_sdk.State() # State | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить отдельный статус CustomerOrder
        api_response = api_instance.update_customer_order_metadata_state_by_id(id, state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->update_customer_order_metadata_state_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->update_customer_order_metadata_state_by_id: %s\n" % e)
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
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_customer_order_note**
> EventNote update_customer_order_note(id, note_id, event_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить Событие Заказа покупателя

Запрос на обновление одного События Заказа покупателя

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.event_note import EventNote
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    note_id = 'note_id_example' # str | ID События
    event_note = moysklad_remap_12_sdk.EventNote() # EventNote | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить Событие Заказа покупателя
        api_response = api_instance.update_customer_order_note(id, note_id, event_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->update_customer_order_note:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->update_customer_order_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **note_id** | **str**| ID События | 
 **event_note** | [**EventNote**](EventNote.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**EventNote**](EventNote.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Событие успешно обновлено |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_customer_order_position**
> CustomerOrderPosition update_customer_order_position(id, position_id, customer_order_position, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Изменить позицию CustomerOrders

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.customer_order_position import CustomerOrderPosition
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
    api_instance = moysklad_remap_12_sdk.CustomerOrdersApi(api_client)
    id = 'id_example' # str | ID сущности
    position_id = 'position_id_example' # str | ID позиции
    customer_order_position = moysklad_remap_12_sdk.CustomerOrderPosition() # CustomerOrderPosition | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    fields = 'fields_example' # str | Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - `minimumStock` — неснижаемый остаток (товар, модификация) - `downloadPermanentHref` — постоянная ссылка на изображение (платный тариф) - `stock` — остатки и себестоимость в позициях документов - `declaration` — прослеживаемость импортных товаров в позициях документов  (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Изменить позицию CustomerOrders
        api_response = api_instance.update_customer_order_position(id, position_id, customer_order_position, expand=expand, fields=fields, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of CustomerOrdersApi->update_customer_order_position:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerOrdersApi->update_customer_order_position: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **position_id** | **str**| ID позиции | 
 **customer_order_position** | [**CustomerOrderPosition**](CustomerOrderPosition.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **fields** | **str**| Включить в ответ скрытые поля, не выводимые по умолчанию. В одном запросе можно передать только одно значение. - &#x60;minimumStock&#x60; — неснижаемый остаток (товар, модификация) - &#x60;downloadPermanentHref&#x60; — постоянная ссылка на изображение (платный тариф) - &#x60;stock&#x60; — остатки и себестоимость в позициях документов - &#x60;declaration&#x60; — прослеживаемость импортных товаров в позициях документов  | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**CustomerOrderPosition**](CustomerOrderPosition.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос |  -  |
**0** | Ошибка запроса (тело — объект или массив объектов с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

