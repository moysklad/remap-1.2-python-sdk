# NotificationRetailShiftOpened

Уведомление об открытии розничной смены

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**retail_store** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**retail_shift** | [**NotificationRetailShift**](NotificationRetailShift.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_retail_shift_opened import NotificationRetailShiftOpened

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationRetailShiftOpened from a JSON string
notification_retail_shift_opened_instance = NotificationRetailShiftOpened.from_json(json)
# print the JSON string representation of the object
print(NotificationRetailShiftOpened.to_json())

# convert the object into a dict
notification_retail_shift_opened_dict = notification_retail_shift_opened_instance.to_dict()
# create an instance of NotificationRetailShiftOpened from a dict
notification_retail_shift_opened_from_dict = NotificationRetailShiftOpened.from_dict(notification_retail_shift_opened_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


