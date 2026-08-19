# CustomEntity

Пользовательский справочник (customentity)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID пользовательского справочника | [optional] [readonly] 
**name** | **str** | Наименование пользовательского справочника | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.custom_entity import CustomEntity

# TODO update the JSON string below
json = "{}"
# create an instance of CustomEntity from a JSON string
custom_entity_instance = CustomEntity.from_json(json)
# print the JSON string representation of the object
print(CustomEntity.to_json())

# convert the object into a dict
custom_entity_dict = custom_entity_instance.to_dict()
# create an instance of CustomEntity from a dict
custom_entity_from_dict = CustomEntity.from_dict(custom_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


