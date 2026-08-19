# VariantCharacteristic

Характеристики модификаций

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID соответствующей Характеристики | [optional] [readonly] 
**name** | **str** | Наименование Характеристики | [optional] 
**type** | **str** | Тип значения Характеристики. Известные значения описаны в VariantCharacteristicType | [optional] [readonly] 
**required** | **bool** | Обязательность указания Характеристики в модификации | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.variant_characteristic import VariantCharacteristic

# TODO update the JSON string below
json = "{}"
# create an instance of VariantCharacteristic from a JSON string
variant_characteristic_instance = VariantCharacteristic.from_json(json)
# print the JSON string representation of the object
print(VariantCharacteristic.to_json())

# convert the object into a dict
variant_characteristic_dict = variant_characteristic_instance.to_dict()
# create an instance of VariantCharacteristic from a dict
variant_characteristic_from_dict = VariantCharacteristic.from_dict(variant_characteristic_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


