# NotificationGroupSettings

Настройки группы уведомлений

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** | Признак активности подписки на группу уведомлений | [optional] 
**channels_enabled** | [**NotificationChannelSettings**](NotificationChannelSettings.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_group_settings import NotificationGroupSettings

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationGroupSettings from a JSON string
notification_group_settings_instance = NotificationGroupSettings.from_json(json)
# print the JSON string representation of the object
print(NotificationGroupSettings.to_json())

# convert the object into a dict
notification_group_settings_dict = notification_group_settings_instance.to_dict()
# create an instance of NotificationGroupSettings from a dict
notification_group_settings_from_dict = NotificationGroupSettings.from_dict(notification_group_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


