# EntityWithMeta

Базовый полиморфный тип для сущностей с `meta`. Конкретный тип определяется по `meta.type`. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.entity_with_meta import EntityWithMeta

# TODO update the JSON string below
json = "{}"
# create an instance of EntityWithMeta from a JSON string
entity_with_meta_instance = EntityWithMeta.from_json(json)
# print the JSON string representation of the object
print(EntityWithMeta.to_json())

# convert the object into a dict
entity_with_meta_dict = entity_with_meta_instance.to_dict()
# create an instance of EntityWithMeta from a dict
entity_with_meta_from_dict = EntityWithMeta.from_dict(entity_with_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


