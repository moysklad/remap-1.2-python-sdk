# NotificationDiffValue

Изменение поля связанного с уведомлением объекта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**old_value** | **str** | Значение поля до изменения | [optional] [readonly] 
**new_value** | **str** | Значение поля после изменения | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_diff_value import NotificationDiffValue

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationDiffValue from a JSON string
notification_diff_value_instance = NotificationDiffValue.from_json(json)
# print the JSON string representation of the object
print(NotificationDiffValue.to_json())

# convert the object into a dict
notification_diff_value_dict = notification_diff_value_instance.to_dict()
# create an instance of NotificationDiffValue from a dict
notification_diff_value_from_dict = NotificationDiffValue.from_dict(notification_diff_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


