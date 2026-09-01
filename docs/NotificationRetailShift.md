# NotificationRetailShift

Краткое представление розничной смены в уведомлении

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID объекта | [optional] 
**name** | **str** | Наименование объекта | [optional] 
**open** | **str** | Дата открытия смены | [optional] 
**close** | **str** | Дата закрытия смены | [optional] 
**proceed** | **int** | Выручка смены | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_retail_shift import NotificationRetailShift

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationRetailShift from a JSON string
notification_retail_shift_instance = NotificationRetailShift.from_json(json)
# print the JSON string representation of the object
print(NotificationRetailShift.to_json())

# convert the object into a dict
notification_retail_shift_dict = notification_retail_shift_instance.to_dict()
# create an instance of NotificationRetailShift from a dict
notification_retail_shift_from_dict = NotificationRetailShift.from_dict(notification_retail_shift_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


