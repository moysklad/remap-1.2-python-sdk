# WebhookAuditContext

Контекст аудита во входящем теле уведомления вебхука (POST на URL подписчика)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**moment** | **str** | Дата изменения | [optional] [readonly] 
**uid** | **str** | Логин сотрудника | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.webhook_audit_context import WebhookAuditContext

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookAuditContext from a JSON string
webhook_audit_context_instance = WebhookAuditContext.from_json(json)
# print the JSON string representation of the object
print(WebhookAuditContext.to_json())

# convert the object into a dict
webhook_audit_context_dict = webhook_audit_context_instance.to_dict()
# create an instance of WebhookAuditContext from a dict
webhook_audit_context_from_dict = WebhookAuditContext.from_dict(webhook_audit_context_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


