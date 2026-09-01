# NotificationSubscribeTermsExpired

Уведомление об истечении условий подписки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**days_left** | **int** | Количество оставшихся дней подписки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_subscribe_terms_expired import NotificationSubscribeTermsExpired

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationSubscribeTermsExpired from a JSON string
notification_subscribe_terms_expired_instance = NotificationSubscribeTermsExpired.from_json(json)
# print the JSON string representation of the object
print(NotificationSubscribeTermsExpired.to_json())

# convert the object into a dict
notification_subscribe_terms_expired_dict = notification_subscribe_terms_expired_instance.to_dict()
# create an instance of NotificationSubscribeTermsExpired from a dict
notification_subscribe_terms_expired_from_dict = NotificationSubscribeTermsExpired.from_dict(notification_subscribe_terms_expired_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


