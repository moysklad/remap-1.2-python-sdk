# SalesManagerChatMessage

Уведомление о новом сообщении от менеджера отдела продаж

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
from moysklad_remap_12_sdk.models.sales_manager_chat_message import SalesManagerChatMessage

# TODO update the JSON string below
json = "{}"
# create an instance of SalesManagerChatMessage from a JSON string
sales_manager_chat_message_instance = SalesManagerChatMessage.from_json(json)
# print the JSON string representation of the object
print(SalesManagerChatMessage.to_json())

# convert the object into a dict
sales_manager_chat_message_dict = sales_manager_chat_message_instance.to_dict()
# create an instance of SalesManagerChatMessage from a dict
sales_manager_chat_message_from_dict = SalesManagerChatMessage.from_dict(sales_manager_chat_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


