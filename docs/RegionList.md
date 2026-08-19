# RegionList

Список регионов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Region]**](Region.md) | Массив регионов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.region_list import RegionList

# TODO update the JSON string below
json = "{}"
# create an instance of RegionList from a JSON string
region_list_instance = RegionList.from_json(json)
# print the JSON string representation of the object
print(RegionList.to_json())

# convert the object into a dict
region_list_dict = region_list_instance.to_dict()
# create an instance of RegionList from a dict
region_list_from_dict = RegionList.from_dict(region_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


