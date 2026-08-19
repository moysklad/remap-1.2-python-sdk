# VariantMetadata

Метаданные модификации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**characteristics** | [**List[VariantCharacteristic]**](VariantCharacteristic.md) | Характеристики Модификации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.variant_metadata import VariantMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of VariantMetadata from a JSON string
variant_metadata_instance = VariantMetadata.from_json(json)
# print the JSON string representation of the object
print(VariantMetadata.to_json())

# convert the object into a dict
variant_metadata_dict = variant_metadata_instance.to_dict()
# create an instance of VariantMetadata from a dict
variant_metadata_from_dict = VariantMetadata.from_dict(variant_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


