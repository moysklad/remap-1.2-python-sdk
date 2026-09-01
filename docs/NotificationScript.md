# NotificationScript

Уведомление из сценария

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_type** | **str** | Тип события сценария. Известные значения описаны в NotificationEventType | [optional] [readonly] 
**entity** | [**NotificationNamedEntity**](NotificationNamedEntity.md) | Объект, на который сработал сценарий | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_script import NotificationScript

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationScript from a JSON string
notification_script_instance = NotificationScript.from_json(json)
# print the JSON string representation of the object
print(NotificationScript.to_json())

# convert the object into a dict
notification_script_dict = notification_script_instance.to_dict()
# create an instance of NotificationScript from a dict
notification_script_from_dict = NotificationScript.from_dict(notification_script_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


