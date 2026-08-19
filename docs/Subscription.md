# Subscription

Подписка компании

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**role** | **str** | Роль авторизованного пользователя (USER/ADMIN) | [optional] [readonly] 
**tariff** | **str** | Действующий тариф Аккаунта. Известные значения описаны в SubscriptionTariff | [optional] [readonly] 
**is_subscription_change_available** | **bool** | Доступность изменения подписки | [optional] [readonly] 
**subscription_end_date** | **int** | Дата (в миллисекундах) окончания действия текущего тарифа, если тариф отличается от \&quot;Пробный\&quot; и \&quot;Бесплатный\&quot; | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.subscription import Subscription

# TODO update the JSON string below
json = "{}"
# create an instance of Subscription from a JSON string
subscription_instance = Subscription.from_json(json)
# print the JSON string representation of the object
print(Subscription.to_json())

# convert the object into a dict
subscription_dict = subscription_instance.to_dict()
# create an instance of Subscription from a dict
subscription_from_dict = Subscription.from_dict(subscription_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


