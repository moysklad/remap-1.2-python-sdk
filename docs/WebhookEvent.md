# WebhookEvent

Элемент массива events во входящем теле уведомления вебхука

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**action** | **str** | Действие, вызвавшее срабатывание. Известные значения описаны в WebhookAction | [optional] 
**account_id** | **str** | ID учетной записи | [optional] 
**updated_fields** | **List[str]** | Поля сущности, измененные пользователем (при diffType&#x3D;FIELDS и action&#x3D;UPDATE у настройки вебхука) | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.webhook_event import WebhookEvent

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEvent from a JSON string
webhook_event_instance = WebhookEvent.from_json(json)
# print the JSON string representation of the object
print(WebhookEvent.to_json())

# convert the object into a dict
webhook_event_dict = webhook_event_instance.to_dict()
# create an instance of WebhookEvent from a dict
webhook_event_from_dict = WebhookEvent.from_dict(webhook_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


