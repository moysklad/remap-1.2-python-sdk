# moysklad_remap_12_sdk.TasksApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_task**](TasksApi.md#create_task) | **POST** /entity/task | Создать задачу
[**create_task_metadata_states**](TasksApi.md#create_task_metadata_states) | **POST** /entity/task/metadata/states | Создать или изменить типы задач
[**create_task_metadata_states_batch**](TasksApi.md#create_task_metadata_states_batch) | **POST** /entity/task/metadata/states/batch | Массовое создание и обновление типов задач
[**create_task_note**](TasksApi.md#create_task_note) | **POST** /entity/task/{id}/notes | Создать комментарий Задачи
[**create_task_notes_batch**](TasksApi.md#create_task_notes_batch) | **POST** /entity/task/{id}/notes/batch | Создать комментарии Задачи
[**create_tasks_batch**](TasksApi.md#create_tasks_batch) | **POST** /entity/task/batch | Создать или изменить задачи
[**delete_task**](TasksApi.md#delete_task) | **DELETE** /entity/task/{id} | Удалить задачу
[**delete_task_metadata_state_by_id**](TasksApi.md#delete_task_metadata_state_by_id) | **DELETE** /entity/task/metadata/states/{id} | Удалить тип задачи
[**delete_task_note**](TasksApi.md#delete_task_note) | **DELETE** /entity/task/{id}/notes/{noteId} | Удалить комментарий к Задаче
[**delete_task_notes_batch**](TasksApi.md#delete_task_notes_batch) | **POST** /entity/task/{id}/notes/delete | Удалить комментарии к Задаче
[**delete_tasks_batch**](TasksApi.md#delete_tasks_batch) | **POST** /entity/task/delete | Удалить задачи
[**get_task_by_id**](TasksApi.md#get_task_by_id) | **GET** /entity/task/{id} | Получить задачу по ID
[**get_task_metadata**](TasksApi.md#get_task_metadata) | **GET** /entity/task/metadata | Получить метаданные задач
[**get_task_note_by_id**](TasksApi.md#get_task_note_by_id) | **GET** /entity/task/{id}/notes/{noteId} | Получить комментарий к Задаче по ID
[**get_task_notes**](TasksApi.md#get_task_notes) | **GET** /entity/task/{id}/notes | Получить комментарии Задачи
[**get_tasks**](TasksApi.md#get_tasks) | **GET** /entity/task | Получить список задач
[**update_task**](TasksApi.md#update_task) | **PUT** /entity/task/{id} | Обновить задачу
[**update_task_metadata_state_by_id**](TasksApi.md#update_task_metadata_state_by_id) | **PUT** /entity/task/metadata/states/{id} | Обновить тип задачи
[**update_task_note**](TasksApi.md#update_task_note) | **PUT** /entity/task/{id}/notes/{noteId} | Обновить комментарий к Задаче


# **create_task**
> Task create_task(task, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать задачу

Создание новой задачи

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task import Task
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    task = moysklad_remap_12_sdk.Task() # Task | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать задачу
        api_response = api_instance.create_task(task, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->create_task:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->create_task: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **task** | [**Task**](Task.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**Task**](Task.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Задача успешно создана |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_task_metadata_states**
> State create_task_metadata_states(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать или изменить типы задач

Создание одного или нескольких типов задач

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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    state = moysklad_remap_12_sdk.State() # State | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать или изменить типы задач
        api_response = api_instance.create_task_metadata_states(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->create_task_metadata_states:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->create_task_metadata_states: %s\n" % e)
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
**200** | Тип задачи или список типов задач успешно обработаны |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_task_metadata_states_batch**
> List[StateRowResult] create_task_metadata_states_batch(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Массовое создание и обновление типов задач

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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    state = [moysklad_remap_12_sdk.State()] # List[State] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Массовое создание и обновление типов задач
        api_response = api_instance.create_task_metadata_states_batch(state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->create_task_metadata_states_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->create_task_metadata_states_batch: %s\n" % e)
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
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_task_note**
> List[TaskNote] create_task_note(id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать комментарий Задачи

Создание комментария к Задаче

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task_note import TaskNote
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    task_note = moysklad_remap_12_sdk.TaskNote() # TaskNote | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать комментарий Задачи
        api_response = api_instance.create_task_note(id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->create_task_note:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->create_task_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **task_note** | [**TaskNote**](TaskNote.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**List[TaskNote]**](TaskNote.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Комментарий успешно создан |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_task_notes_batch**
> List[BatchResponseEntity] create_task_notes_batch(id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать комментарии Задачи

Создание нескольких комментариев к Задаче.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.batch_response_entity import BatchResponseEntity
from moysklad_remap_12_sdk.models.task_note import TaskNote
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    task_note = [moysklad_remap_12_sdk.TaskNote()] # List[TaskNote] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать комментарии Задачи
        api_response = api_instance.create_task_notes_batch(id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->create_task_notes_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->create_task_notes_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **task_note** | [**List[TaskNote]**](TaskNote.md)|  | 
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
**200** | Комментарии успешно созданы |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_tasks_batch**
> List[BatchResponseEntity] create_tasks_batch(task, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Создать или изменить задачи

Создание или изменение нескольких задач.

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.batch_response_entity import BatchResponseEntity
from moysklad_remap_12_sdk.models.task import Task
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    task = [moysklad_remap_12_sdk.Task()] # List[Task] | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Создать или изменить задачи
        api_response = api_instance.create_tasks_batch(task, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->create_tasks_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->create_tasks_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **task** | [**List[Task]**](Task.md)|  | 
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
**200** | Задачи созданы или изменены (элемент — сущность или объект ошибки) |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_task**
> delete_task(id, accept=accept, accept_encoding=accept_encoding)

Удалить задачу

Удаление задачи с указанным id

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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить задачу
        api_instance.delete_task(id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling TasksApi->delete_task: %s\n" % e)
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
**200** | Задача успешно удалена |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_task_metadata_state_by_id**
> delete_task_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить тип задачи

Удаление типа задачи с указанным id

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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить тип задачи
        api_instance.delete_task_metadata_state_by_id(id, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling TasksApi->delete_task_metadata_state_by_id: %s\n" % e)
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
**200** | Тип задачи успешно удален |  -  |
**404** | Запрошенный ресурс не существует (тело ответа отсутствует) |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_task_note**
> delete_task_note(id, note_id, accept=accept, accept_encoding=accept_encoding)

Удалить комментарий к Задаче

Удаление комментария к Задаче с указанным id

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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    note_id = 'note_id_example' # str | ID комментария к Задаче
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Удалить комментарий к Задаче
        api_instance.delete_task_note(id, note_id, accept=accept, accept_encoding=accept_encoding)
    except Exception as e:
        print("Exception when calling TasksApi->delete_task_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **note_id** | **str**| ID комментария к Задаче | 
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
**200** | Комментарий успешно удален |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_task_notes_batch**
> delete_task_notes_batch(id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить комментарии к Задаче

Массовое удаление комментариев к Задаче по их мета-объектам

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task_note import TaskNote
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    task_note = [moysklad_remap_12_sdk.TaskNote()] # List[TaskNote] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить комментарии к Задаче
        api_instance.delete_task_notes_batch(id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
    except Exception as e:
        print("Exception when calling TasksApi->delete_task_notes_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **task_note** | [**List[TaskNote]**](TaskNote.md)|  | 
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
**200** | Комментарии к Задаче успешно удалены |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_tasks_batch**
> List[DeleteRowResult] delete_tasks_batch(task, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Удалить задачи

Массовое удаление задач по их мета-объектам

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.delete_row_result import DeleteRowResult
from moysklad_remap_12_sdk.models.task import Task
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    task = [moysklad_remap_12_sdk.Task()] # List[Task] | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Удалить задачи
        api_response = api_instance.delete_tasks_batch(task, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->delete_tasks_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->delete_tasks_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **task** | [**List[Task]**](Task.md)|  | 
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

# **get_task_by_id**
> Task get_task_by_id(id, expand=expand, accept=accept, accept_encoding=accept_encoding)

Получить задачу по ID

Запрос задачи с указанным id

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task import Task
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить задачу по ID
        api_response = api_instance.get_task_by_id(id, expand=expand, accept=accept, accept_encoding=accept_encoding)
        print("The response of TasksApi->get_task_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->get_task_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**Task**](Task.md)

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

# **get_task_metadata**
> DocumentMetadata get_task_metadata(accept=accept, accept_encoding=accept_encoding)

Получить метаданные задач

Запрос на получение метаданных задач

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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить метаданные задач
        api_response = api_instance.get_task_metadata(accept=accept, accept_encoding=accept_encoding)
        print("The response of TasksApi->get_task_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->get_task_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

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

# **get_task_note_by_id**
> TaskNote get_task_note_by_id(id, note_id, accept=accept, accept_encoding=accept_encoding)

Получить комментарий к Задаче по ID

Запрос на получение отдельного комментария к Задаче с указанным id

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task_note import TaskNote
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    note_id = 'note_id_example' # str | ID комментария к Задаче
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить комментарий к Задаче по ID
        api_response = api_instance.get_task_note_by_id(id, note_id, accept=accept, accept_encoding=accept_encoding)
        print("The response of TasksApi->get_task_note_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->get_task_note_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **note_id** | **str**| ID комментария к Задаче | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**TaskNote**](TaskNote.md)

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

# **get_task_notes**
> TaskNoteList get_task_notes(id, limit=limit, offset=offset, updated_by=updated_by, updated_from=updated_from, updated_to=updated_to, accept=accept, accept_encoding=accept_encoding)

Получить комментарии Задачи

Запрос на получение списка всех комментариев данной Задачи

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task_note_list import TaskNoteList
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    updated_by = 'updated_by_example' # str | Автор последнего обновления (uid, используется для фильтрации) (optional)
    updated_from = 'updated_from_example' # str | Нижняя граница даты обновления в формате YYYY-MM-DD HH:MM:SS[.mmm] (optional)
    updated_to = 'updated_to_example' # str | Верхняя граница даты обновления в формате YYYY-MM-DD HH:MM:SS[.mmm] (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить комментарии Задачи
        api_response = api_instance.get_task_notes(id, limit=limit, offset=offset, updated_by=updated_by, updated_from=updated_from, updated_to=updated_to, accept=accept, accept_encoding=accept_encoding)
        print("The response of TasksApi->get_task_notes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->get_task_notes: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **updated_by** | **str**| Автор последнего обновления (uid, используется для фильтрации) | [optional] 
 **updated_from** | **str**| Нижняя граница даты обновления в формате YYYY-MM-DD HH:MM:SS[.mmm] | [optional] 
 **updated_to** | **str**| Верхняя граница даты обновления в формате YYYY-MM-DD HH:MM:SS[.mmm] | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**TaskNoteList**](TaskNoteList.md)

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

# **get_tasks**
> TaskList get_tasks(limit=limit, offset=offset, filter=filter, expand=expand, order=order, accept=accept, accept_encoding=accept_encoding)

Получить список задач

Запрос всех задач на данной учетной записи

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task_list import TaskList
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    limit = 1000 # int | Максимальное количество элементов в выданном списке (максимум 1000) (optional) (default to 1000)
    offset = 0 # int | Отступ в выданном списке (optional) (default to 0)
    filter = 'filter_example' # str | Фильтрация выборки (optional)
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    order = 'order_example' # str | Сортировка (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить список задач
        api_response = api_instance.get_tasks(limit=limit, offset=offset, filter=filter, expand=expand, order=order, accept=accept, accept_encoding=accept_encoding)
        print("The response of TasksApi->get_tasks:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->get_tasks: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Максимальное количество элементов в выданном списке (максимум 1000) | [optional] [default to 1000]
 **offset** | **int**| Отступ в выданном списке | [optional] [default to 0]
 **filter** | **str**| Фильтрация выборки | [optional] 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **order** | **str**| Сортировка | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**TaskList**](TaskList.md)

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

# **update_task**
> Task update_task(id, task, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить задачу

Обновление задачи с указанным id

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task import Task
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    task = moysklad_remap_12_sdk.Task() # Task | 
    expand = 'expand_example' # str | Замена ссылок объектами с помощью expand (optional)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить задачу
        api_response = api_instance.update_task(id, task, expand=expand, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->update_task:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->update_task: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **task** | [**Task**](Task.md)|  | 
 **expand** | **str**| Замена ссылок объектами с помощью expand | [optional] 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**Task**](Task.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Задача успешно обновлена |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_task_metadata_state_by_id**
> State update_task_metadata_state_by_id(id, state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить тип задачи

Обновление типа задачи с указанным id

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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    state = moysklad_remap_12_sdk.State() # State | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить тип задачи
        api_response = api_instance.update_task_metadata_state_by_id(id, state, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->update_task_metadata_state_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->update_task_metadata_state_by_id: %s\n" % e)
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
**200** | Тип задачи успешно обновлен |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_task_note**
> TaskNote update_task_note(id, note_id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)

Обновить комментарий к Задаче

Обновление комментария к Задаче с указанным id

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.task_note import TaskNote
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
    api_instance = moysklad_remap_12_sdk.TasksApi(api_client)
    id = 'id_example' # str | ID сущности
    note_id = 'note_id_example' # str | ID комментария к Задаче
    task_note = moysklad_remap_12_sdk.TaskNote() # TaskNote | 
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')
    content_type = application/json # str |  (optional) (default to application/json)

    try:
        # Обновить комментарий к Задаче
        api_response = api_instance.update_task_note(id, note_id, task_note, accept=accept, accept_encoding=accept_encoding, content_type=content_type)
        print("The response of TasksApi->update_task_note:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TasksApi->update_task_note: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ID сущности | 
 **note_id** | **str**| ID комментария к Задаче | 
 **task_note** | [**TaskNote**](TaskNote.md)|  | 
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]
 **content_type** | **str**|  | [optional] [default to application/json]

### Return type

[**TaskNote**](TaskNote.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Комментарий успешно обновлен |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

