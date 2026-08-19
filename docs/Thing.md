# Thing

Серийный номер

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Серийного номера | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Значение серийного номера | [optional] 
**description** | **str** | Комментарий к серийному номеру | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.thing import Thing

# TODO update the JSON string below
json = "{}"
# create an instance of Thing from a JSON string
thing_instance = Thing.from_json(json)
# print the JSON string representation of the object
print(Thing.to_json())

# convert the object into a dict
thing_dict = thing_instance.to_dict()
# create an instance of Thing from a dict
thing_from_dict = Thing.from_dict(thing_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


