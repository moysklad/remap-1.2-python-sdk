# NotificationGoodCountTooLow

Уведомление о снижении остатка товара ниже неснижаемого

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**actual_balance** | **float** | Остаток товара | [optional] 
**good** | [**NotificationNamedEntity**](NotificationNamedEntity.md) |  | [optional] 
**minimum_balance** | **float** | Неснижаемый остаток товара | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_good_count_too_low import NotificationGoodCountTooLow

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationGoodCountTooLow from a JSON string
notification_good_count_too_low_instance = NotificationGoodCountTooLow.from_json(json)
# print the JSON string representation of the object
print(NotificationGoodCountTooLow.to_json())

# convert the object into a dict
notification_good_count_too_low_dict = notification_good_count_too_low_instance.to_dict()
# create an instance of NotificationGoodCountTooLow from a dict
notification_good_count_too_low_from_dict = NotificationGoodCountTooLow.from_dict(notification_good_count_too_low_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


