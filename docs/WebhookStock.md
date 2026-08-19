# WebhookStock

Вебхук на изменение остатков

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID вебхука на изменение остатков | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**stock_type** | **str** | Тип остатков. Известные значения описаны в WebhookStockStockType | [optional] 
**report_type** | **str** | Тип отчёта остатков. Известные значения описаны в WebhookStockReportType | [optional] 
**url** | **str** | URL, по которому будет происходить обработка вебхука | [optional] 
**enabled** | **bool** | Вебхук включён или отключён | [optional] 
**author_application** | [**Application**](Application.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.webhook_stock import WebhookStock

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookStock from a JSON string
webhook_stock_instance = WebhookStock.from_json(json)
# print the JSON string representation of the object
print(WebhookStock.to_json())

# convert the object into a dict
webhook_stock_dict = webhook_stock_instance.to_dict()
# create an instance of WebhookStock from a dict
webhook_stock_from_dict = WebhookStock.from_dict(webhook_stock_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


