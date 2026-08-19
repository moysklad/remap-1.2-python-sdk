# NotificationSettings

Настройки уведомлений текущего пользователя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_order** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**data_exchange** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**invoice** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**retail** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**scripts** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**stock** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**task** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**mentions** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**online_stores** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 
**followed_events** | [**NotificationGroupSettings**](NotificationGroupSettings.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_settings import NotificationSettings

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationSettings from a JSON string
notification_settings_instance = NotificationSettings.from_json(json)
# print the JSON string representation of the object
print(NotificationSettings.to_json())

# convert the object into a dict
notification_settings_dict = notification_settings_instance.to_dict()
# create an instance of NotificationSettings from a dict
notification_settings_from_dict = NotificationSettings.from_dict(notification_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


