# NotificationNamedEntity

Краткое представление связанного с уведомлением объекта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID объекта | [optional] 
**name** | **str** | Наименование объекта | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.notification_named_entity import NotificationNamedEntity

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationNamedEntity from a JSON string
notification_named_entity_instance = NotificationNamedEntity.from_json(json)
# print the JSON string representation of the object
print(NotificationNamedEntity.to_json())

# convert the object into a dict
notification_named_entity_dict = notification_named_entity_instance.to_dict()
# create an instance of NotificationNamedEntity from a dict
notification_named_entity_from_dict = NotificationNamedEntity.from_dict(notification_named_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


