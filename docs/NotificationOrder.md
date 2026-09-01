# NotificationOrder

Краткое представление заказа покупателя в уведомлении

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID объекта | [optional] 
**name** | **str** | Наименование объекта | [optional] 
**agent_name** | **str** | Имя контрагента | [optional] 
**delivery_planned_moment** | **str** | Планируемое время отгрузки | [optional] 
**sum** | **int** | Сумма заказа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_order import NotificationOrder

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationOrder from a JSON string
notification_order_instance = NotificationOrder.from_json(json)
# print the JSON string representation of the object
print(NotificationOrder.to_json())

# convert the object into a dict
notification_order_dict = notification_order_instance.to_dict()
# create an instance of NotificationOrder from a dict
notification_order_from_dict = NotificationOrder.from_dict(notification_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


