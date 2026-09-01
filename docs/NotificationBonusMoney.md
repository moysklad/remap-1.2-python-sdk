# NotificationBonusMoney

Уведомление о зачислении бонусных денег

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
from moysklad_remap_12_sdk.models.notification_bonus_money import NotificationBonusMoney

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationBonusMoney from a JSON string
notification_bonus_money_instance = NotificationBonusMoney.from_json(json)
# print the JSON string representation of the object
print(NotificationBonusMoney.to_json())

# convert the object into a dict
notification_bonus_money_dict = notification_bonus_money_instance.to_dict()
# create an instance of NotificationBonusMoney from a dict
notification_bonus_money_from_dict = NotificationBonusMoney.from_dict(notification_bonus_money_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


