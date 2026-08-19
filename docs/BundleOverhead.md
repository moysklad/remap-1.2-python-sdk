# BundleOverhead

Дополнительные расходы

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **float** | Значение цены | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bundle_overhead import BundleOverhead

# TODO update the JSON string below
json = "{}"
# create an instance of BundleOverhead from a JSON string
bundle_overhead_instance = BundleOverhead.from_json(json)
# print the JSON string representation of the object
print(BundleOverhead.to_json())

# convert the object into a dict
bundle_overhead_dict = bundle_overhead_instance.to_dict()
# create an instance of BundleOverhead from a dict
bundle_overhead_from_dict = BundleOverhead.from_dict(bundle_overhead_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


