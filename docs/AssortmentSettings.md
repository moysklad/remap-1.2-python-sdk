# AssortmentSettings

Настройки ассортимента

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**barcode_rules** | [**AssortmentSettingsBarcodeRules**](AssortmentSettingsBarcodeRules.md) |  | [optional] 
**unique_code_rules** | [**AssortmentSettingsUniqueCodeRules**](AssortmentSettingsUniqueCodeRules.md) |  | [optional] 
**created_shared** | **bool** | Создавать новые элементы с меткой \&quot;Общий\&quot; | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.assortment_settings import AssortmentSettings

# TODO update the JSON string below
json = "{}"
# create an instance of AssortmentSettings from a JSON string
assortment_settings_instance = AssortmentSettings.from_json(json)
# print the JSON string representation of the object
print(AssortmentSettings.to_json())

# convert the object into a dict
assortment_settings_dict = assortment_settings_instance.to_dict()
# create an instance of AssortmentSettings from a dict
assortment_settings_from_dict = AssortmentSettings.from_dict(assortment_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


