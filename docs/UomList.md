# UomList

Список единиц измерения

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Uom]**](Uom.md) | Массив единиц измерения | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.uom_list import UomList

# TODO update the JSON string below
json = "{}"
# create an instance of UomList from a JSON string
uom_list_instance = UomList.from_json(json)
# print the JSON string representation of the object
print(UomList.to_json())

# convert the object into a dict
uom_list_dict = uom_list_instance.to_dict()
# create an instance of UomList from a dict
uom_list_from_dict = UomList.from_dict(uom_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


