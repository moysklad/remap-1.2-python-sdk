# WebhookStockList

Список вебхуков на изменение остатков

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[WebhookStock]**](WebhookStock.md) | Массив вебхуков на изменение остатков | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.webhook_stock_list import WebhookStockList

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookStockList from a JSON string
webhook_stock_list_instance = WebhookStockList.from_json(json)
# print the JSON string representation of the object
print(WebhookStockList.to_json())

# convert the object into a dict
webhook_stock_list_dict = webhook_stock_list_instance.to_dict()
# create an instance of WebhookStockList from a dict
webhook_stock_list_from_dict = WebhookStockList.from_dict(webhook_stock_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


