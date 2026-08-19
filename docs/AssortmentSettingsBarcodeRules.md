# AssortmentSettingsBarcodeRules

Настройки правил штрихкодов для сущностей ассортимента

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fill_ean13_barcode** | **bool** | Автоматически создавать штрихкод EAN13 | [optional] 
**weight_barcode** | **bool** | Использовать префиксы штрихкодов для весовых товаров | [optional] 
**weight_barcode_prefix** | **int** | Префикс штрихкодов для весовых товаров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.assortment_settings_barcode_rules import AssortmentSettingsBarcodeRules

# TODO update the JSON string below
json = "{}"
# create an instance of AssortmentSettingsBarcodeRules from a JSON string
assortment_settings_barcode_rules_instance = AssortmentSettingsBarcodeRules.from_json(json)
# print the JSON string representation of the object
print(AssortmentSettingsBarcodeRules.to_json())

# convert the object into a dict
assortment_settings_barcode_rules_dict = assortment_settings_barcode_rules_instance.to_dict()
# create an instance of AssortmentSettingsBarcodeRules from a dict
assortment_settings_barcode_rules_from_dict = AssortmentSettingsBarcodeRules.from_dict(assortment_settings_barcode_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


