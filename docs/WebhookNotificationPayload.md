# WebhookNotificationPayload

Тело HTTP POST, которое МойСклад отправляет на url вебхука при событии. Параметр query requestId идентифицирует уведомление (сохраняется при повторных попытках). 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**audit_context** | [**WebhookAuditContext**](WebhookAuditContext.md) |  | [optional] 
**events** | [**List[WebhookEvent]**](WebhookEvent.md) | Данные о событии или нескольких событиях | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.webhook_notification_payload import WebhookNotificationPayload

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookNotificationPayload from a JSON string
webhook_notification_payload_instance = WebhookNotificationPayload.from_json(json)
# print the JSON string representation of the object
print(WebhookNotificationPayload.to_json())

# convert the object into a dict
webhook_notification_payload_dict = webhook_notification_payload_instance.to_dict()
# create an instance of WebhookNotificationPayload from a dict
webhook_notification_payload_from_dict = WebhookNotificationPayload.from_dict(webhook_notification_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


