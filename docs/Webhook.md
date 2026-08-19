# Webhook

Вебхук

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID вебхука | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**entity_type** | **str** | Тип сущности, к которой привязан вебхук. Известные ограничения см. в документации (нельзя webhook, discount, notes) | [optional] 
**url** | **str** | URL, по которому отправляется уведомление | [optional] 
**method** | **str** | HTTP метод запроса к URL подписчика. Известные значения описаны в WebhookMethod | [optional] 
**enabled** | **bool** | Вебхук включен или отключен | [optional] 
**action** | **str** | Отслеживаемое действие. Известные значения описаны в WebhookAction. Значение PROCESSED допустимо только для асинхронных задач | [optional] 
**diff_type** | **str** | Режим для действия UPDATE. Известные значения описаны в WebhookDiffType | [optional] 
**author_application** | [**Application**](Application.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.webhook import Webhook

# TODO update the JSON string below
json = "{}"
# create an instance of Webhook from a JSON string
webhook_instance = Webhook.from_json(json)
# print the JSON string representation of the object
print(Webhook.to_json())

# convert the object into a dict
webhook_dict = webhook_instance.to_dict()
# create an instance of Webhook from a dict
webhook_from_dict = Webhook.from_dict(webhook_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


