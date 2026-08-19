# BundleList

Список комплектов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Bundle]**](Bundle.md) | Массив комплектов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bundle_list import BundleList

# TODO update the JSON string below
json = "{}"
# create an instance of BundleList from a JSON string
bundle_list_instance = BundleList.from_json(json)
# print the JSON string representation of the object
print(BundleList.to_json())

# convert the object into a dict
bundle_list_dict = bundle_list_instance.to_dict()
# create an instance of BundleList from a dict
bundle_list_from_dict = BundleList.from_dict(bundle_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


