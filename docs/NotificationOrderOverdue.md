# NotificationOrderOverdue

Уведомление о просроченном заказе покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**agent_name** | **str** | Имя контрагента | [optional] 
**delivery_planned_moment** | **str** | Планируемое время отгрузки | [optional] 
**order** | [**NotificationOrder**](NotificationOrder.md) |  | [optional] 
**sum** | **int** | Сумма заказа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_order_overdue import NotificationOrderOverdue

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationOrderOverdue from a JSON string
notification_order_overdue_instance = NotificationOrderOverdue.from_json(json)
# print the JSON string representation of the object
print(NotificationOrderOverdue.to_json())

# convert the object into a dict
notification_order_overdue_dict = notification_order_overdue_instance.to_dict()
# create an instance of NotificationOrderOverdue from a dict
notification_order_overdue_from_dict = NotificationOrderOverdue.from_dict(notification_order_overdue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


