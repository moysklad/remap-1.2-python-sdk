# ErrorErrorsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** | Заголовок ошибки | 
**parameter** | **str** | Параметр, на котором произошла ошибка | [optional] 
**code** | **int** | Код ошибки | [optional] 
**error_message** | **str** | Сообщение, прилагаемое к ошибке | [optional] 
**more_info** | **str** | Ссылка на документацию с описанием ошибки | [optional] 
**line** | **int** | Строка JSON, на которой произошла ошибка | [optional] 
**column** | **int** | Координата элемента в строке, на котором произошла ошибка | [optional] 
**dependencies** | [**List[Meta]**](Meta.md) | Список метаданных зависимых сущностей | [optional] 
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.error_errors_inner import ErrorErrorsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ErrorErrorsInner from a JSON string
error_errors_inner_instance = ErrorErrorsInner.from_json(json)
# print the JSON string representation of the object
print(ErrorErrorsInner.to_json())

# convert the object into a dict
error_errors_inner_dict = error_errors_inner_instance.to_dict()
# create an instance of ErrorErrorsInner from a dict
error_errors_inner_from_dict = ErrorErrorsInner.from_dict(error_errors_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


