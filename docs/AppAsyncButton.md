# AppAsyncButton

Уведомление об окончании обработки нажатия асинхронной кастомной кнопки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID уведомления | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**created** | **str** | Дата и время формирования уведомления | [optional] [readonly] 
**read** | **bool** | Признак того, было ли уведомление прочитано | [optional] 
**title** | **str** | Краткий текст уведомления | [optional] [readonly] 
**description** | **str** | Описание уведомления | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.app_async_button import AppAsyncButton

# TODO update the JSON string below
json = "{}"
# create an instance of AppAsyncButton from a JSON string
app_async_button_instance = AppAsyncButton.from_json(json)
# print the JSON string representation of the object
print(AppAsyncButton.to_json())

# convert the object into a dict
app_async_button_dict = app_async_button_instance.to_dict()
# create an instance of AppAsyncButton from a dict
app_async_button_from_dict = AppAsyncButton.from_dict(app_async_button_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


