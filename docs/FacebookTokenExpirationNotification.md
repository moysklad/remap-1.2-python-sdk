# FacebookTokenExpirationNotification

Уведомление об окончании доступа к аккаунту Facebook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**connector_name** | **str** | Название коннектора | [optional] 
**days_left_to_expiration** | **int** | Количество дней до окончания доступа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.facebook_token_expiration_notification import FacebookTokenExpirationNotification

# TODO update the JSON string below
json = "{}"
# create an instance of FacebookTokenExpirationNotification from a JSON string
facebook_token_expiration_notification_instance = FacebookTokenExpirationNotification.from_json(json)
# print the JSON string representation of the object
print(FacebookTokenExpirationNotification.to_json())

# convert the object into a dict
facebook_token_expiration_notification_dict = facebook_token_expiration_notification_instance.to_dict()
# create an instance of FacebookTokenExpirationNotification from a dict
facebook_token_expiration_notification_from_dict = FacebookTokenExpirationNotification.from_dict(facebook_token_expiration_notification_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


