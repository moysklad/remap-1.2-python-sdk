# BundleComponentList

Список элементов комплекта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[BundleComponent]**](BundleComponent.md) | Массив элементов комплекта | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bundle_component_list import BundleComponentList

# TODO update the JSON string below
json = "{}"
# create an instance of BundleComponentList from a JSON string
bundle_component_list_instance = BundleComponentList.from_json(json)
# print the JSON string representation of the object
print(BundleComponentList.to_json())

# convert the object into a dict
bundle_component_list_dict = bundle_component_list_instance.to_dict()
# create an instance of BundleComponentList from a dict
bundle_component_list_from_dict = BundleComponentList.from_dict(bundle_component_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


