# NotificationOrderNew

Уведомление о новом заказе покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**agent_name** | **str** | Имя контрагента | [optional] 
**delivery_planned_moment** | **str** | Планируемое время отгрузки | [optional] 
**order** | [**NotificationOrder**](NotificationOrder.md) |  | [optional] 
**sum** | **int** | Сумма заказа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_order_new import NotificationOrderNew

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationOrderNew from a JSON string
notification_order_new_instance = NotificationOrderNew.from_json(json)
# print the JSON string representation of the object
print(NotificationOrderNew.to_json())

# convert the object into a dict
notification_order_new_dict = notification_order_new_instance.to_dict()
# create an instance of NotificationOrderNew from a dict
notification_order_new_from_dict = NotificationOrderNew.from_dict(notification_order_new_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


