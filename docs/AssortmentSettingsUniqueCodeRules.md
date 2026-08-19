# AssortmentSettingsUniqueCodeRules

Настройки уникальности кода для сущностей ассортимента

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**check_unique_code** | **bool** | Проверка уникальности кода сущностей ассортимента | [optional] 
**fill_unique_code** | **bool** | Устанавливать уникальный код при создании сущностей ассортимента | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.assortment_settings_unique_code_rules import AssortmentSettingsUniqueCodeRules

# TODO update the JSON string below
json = "{}"
# create an instance of AssortmentSettingsUniqueCodeRules from a JSON string
assortment_settings_unique_code_rules_instance = AssortmentSettingsUniqueCodeRules.from_json(json)
# print the JSON string representation of the object
print(AssortmentSettingsUniqueCodeRules.to_json())

# convert the object into a dict
assortment_settings_unique_code_rules_dict = assortment_settings_unique_code_rules_instance.to_dict()
# create an instance of AssortmentSettingsUniqueCodeRules from a dict
assortment_settings_unique_code_rules_from_dict = AssortmentSettingsUniqueCodeRules.from_dict(assortment_settings_unique_code_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


