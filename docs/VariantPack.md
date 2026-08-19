# VariantPack

Упаковка модификации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID упаковки | [optional] [readonly] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды упаковки модификации | [optional] 
**parentpack** | [**Pack**](Pack.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.variant_pack import VariantPack

# TODO update the JSON string below
json = "{}"
# create an instance of VariantPack from a JSON string
variant_pack_instance = VariantPack.from_json(json)
# print the JSON string representation of the object
print(VariantPack.to_json())

# convert the object into a dict
variant_pack_dict = variant_pack_instance.to_dict()
# create an instance of VariantPack from a dict
variant_pack_from_dict = VariantPack.from_dict(variant_pack_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


