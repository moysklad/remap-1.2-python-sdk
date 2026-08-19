# VariantCharacteristicValue

Значение характеристики модификаций

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID соответствующей Характеристики | [optional] [readonly] 
**name** | **str** | Наименование Характеристики | [optional] 
**value** | **str** | Значение Характеристики | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.variant_characteristic_value import VariantCharacteristicValue

# TODO update the JSON string below
json = "{}"
# create an instance of VariantCharacteristicValue from a JSON string
variant_characteristic_value_instance = VariantCharacteristicValue.from_json(json)
# print the JSON string representation of the object
print(VariantCharacteristicValue.to_json())

# convert the object into a dict
variant_characteristic_value_dict = variant_characteristic_value_instance.to_dict()
# create an instance of VariantCharacteristicValue from a dict
variant_characteristic_value_from_dict = VariantCharacteristicValue.from_dict(variant_characteristic_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


