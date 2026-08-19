# VariantList

Список Модификаций

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Variant]**](Variant.md) | Массив Модификаций | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.variant_list import VariantList

# TODO update the JSON string below
json = "{}"
# create an instance of VariantList from a JSON string
variant_list_instance = VariantList.from_json(json)
# print the JSON string representation of the object
print(VariantList.to_json())

# convert the object into a dict
variant_list_dict = variant_list_instance.to_dict()
# create an instance of VariantList from a dict
variant_list_from_dict = VariantList.from_dict(variant_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


