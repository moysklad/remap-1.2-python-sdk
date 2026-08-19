# ThingList

Список Серийных номеров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Thing]**](Thing.md) | Массив Серийных номеров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.thing_list import ThingList

# TODO update the JSON string below
json = "{}"
# create an instance of ThingList from a JSON string
thing_list_instance = ThingList.from_json(json)
# print the JSON string representation of the object
print(ThingList.to_json())

# convert the object into a dict
thing_list_dict = thing_list_instance.to_dict()
# create an instance of ThingList from a dict
thing_list_from_dict = ThingList.from_dict(thing_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


