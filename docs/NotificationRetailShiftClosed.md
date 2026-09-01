# NotificationRetailShiftClosed

Уведомление о закрытии розничной смены

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**retail_store** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**retail_shift** | [**NotificationRetailShift**](NotificationRetailShift.md) |  | [optional] 
**returns** | **int** | Количество возвратов | [optional] 
**sales** | **int** | Количество продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_retail_shift_closed import NotificationRetailShiftClosed

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationRetailShiftClosed from a JSON string
notification_retail_shift_closed_instance = NotificationRetailShiftClosed.from_json(json)
# print the JSON string representation of the object
print(NotificationRetailShiftClosed.to_json())

# convert the object into a dict
notification_retail_shift_closed_dict = notification_retail_shift_closed_instance.to_dict()
# create an instance of NotificationRetailShiftClosed from a dict
notification_retail_shift_closed_from_dict = NotificationRetailShiftClosed.from_dict(notification_retail_shift_closed_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


