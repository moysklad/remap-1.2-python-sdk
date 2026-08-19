# WebhookStockNotificationPayload

Тело HTTP POST, которое МойСклад отправляет на url вебхука при изменении остатков (уведомления с интервалом 1–5 минут). Параметр query requestId идентифицирует уведомление (сохраняется при повторных попытках). 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** | ID учетной записи | [optional] 
**stock_type** | **str** | Тип остатков. Известные значения описаны в WebhookStockStockType | [optional] 
**report_type** | **str** | Тип отчёта. Известные значения описаны в WebhookStockReportType | [optional] 
**report_url** | **str** | URL для получения данных по изменившейся номенклатуре за период (отчёт об остатках) | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.webhook_stock_notification_payload import WebhookStockNotificationPayload

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookStockNotificationPayload from a JSON string
webhook_stock_notification_payload_instance = WebhookStockNotificationPayload.from_json(json)
# print the JSON string representation of the object
print(WebhookStockNotificationPayload.to_json())

# convert the object into a dict
webhook_stock_notification_payload_dict = webhook_stock_notification_payload_instance.to_dict()
# create an instance of WebhookStockNotificationPayload from a dict
webhook_stock_notification_payload_from_dict = WebhookStockNotificationPayload.from_dict(webhook_stock_notification_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


