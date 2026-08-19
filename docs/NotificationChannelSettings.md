# NotificationChannelSettings

Настройки каналов доставки уведомлений

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **bool** | Признак активности доставки уведомлений по электронной почте | [optional] 
**push** | **bool** | Признак активности доставки уведомлений через мобильные push-уведомления | [optional] 
**interface** | **bool** | Признак активности доставки уведомлений в веб-интерфейсе | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_channel_settings import NotificationChannelSettings

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationChannelSettings from a JSON string
notification_channel_settings_instance = NotificationChannelSettings.from_json(json)
# print the JSON string representation of the object
print(NotificationChannelSettings.to_json())

# convert the object into a dict
notification_channel_settings_dict = notification_channel_settings_instance.to_dict()
# create an instance of NotificationChannelSettings from a dict
notification_channel_settings_from_dict = NotificationChannelSettings.from_dict(notification_channel_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


