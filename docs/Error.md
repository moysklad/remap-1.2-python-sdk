# Error


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
from moysklad_remap_12_sdk.models.error import Error

# TODO update the JSON string below
json = "{}"
# create an instance of Error from a JSON string
error_instance = Error.from_json(json)
# print the JSON string representation of the object
print(Error.to_json())

# convert the object into a dict
error_dict = error_instance.to_dict()
# create an instance of Error from a dict
error_from_dict = Error.from_dict(error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


