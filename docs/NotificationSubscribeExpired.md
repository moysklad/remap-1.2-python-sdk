# NotificationSubscribeExpired

Уведомление об окончании подписки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID уведомления | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**created** | **str** | Дата и время формирования уведомления | [optional] [readonly] 
**read** | **bool** | Признак того, было ли уведомление прочитано | [optional] 
**title** | **str** | Краткий текст уведомления | [optional] [readonly] 
**description** | **str** | Описание уведомления | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_subscribe_expired import NotificationSubscribeExpired

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationSubscribeExpired from a JSON string
notification_subscribe_expired_instance = NotificationSubscribeExpired.from_json(json)
# print the JSON string representation of the object
print(NotificationSubscribeExpired.to_json())

# convert the object into a dict
notification_subscribe_expired_dict = notification_subscribe_expired_instance.to_dict()
# create an instance of NotificationSubscribeExpired from a dict
notification_subscribe_expired_from_dict = NotificationSubscribeExpired.from_dict(notification_subscribe_expired_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


