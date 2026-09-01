# moysklad_remap_12_sdk.SubscriptionsApi

All URIs are relative to *https://api.moysklad.ru/api/remap/1.2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_subscription**](SubscriptionsApi.md#get_subscription) | **GET** /accountSettings/subscription | Получить Подписку компании


# **get_subscription**
> Subscription get_subscription(accept=accept, accept_encoding=accept_encoding)

Получить Подписку компании

Запрос на получение действующей подписки компании

### Example

* Basic Authentication (basicAuth):
* Bearer Authentication (bearerAuth):

```python
import moysklad_remap_12_sdk
from moysklad_remap_12_sdk.models.subscription import Subscription
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
    api_instance = moysklad_remap_12_sdk.SubscriptionsApi(api_client)
    accept = application/json;charset=utf-8 # str |  (optional) (default to application/json;charset=utf-8)
    accept_encoding = 'gzip, deflate, br' # str |  (optional) (default to 'gzip, deflate, br')

    try:
        # Получить Подписку компании
        api_response = api_instance.get_subscription(accept=accept, accept_encoding=accept_encoding)
        print("The response of SubscriptionsApi->get_subscription:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->get_subscription: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept** | **str**|  | [optional] [default to application/json;charset&#x3D;utf-8]
 **accept_encoding** | **str**|  | [optional] [default to &#39;gzip, deflate, br&#39;]

### Return type

[**Subscription**](Subscription.md)

### Authorization

[basicAuth](../README.md#basicAuth), [bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html;charset=UTF-8

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Успешный запрос. Результат - JSON представление Подписки компании |  -  |
**0** | Ошибка запроса (тело — объект с полем errors) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

