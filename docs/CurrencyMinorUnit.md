# CurrencyMinorUnit

Форма разменной единицы

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gender** | **str** | Пол. Известные значения описаны в Gender | [optional] 
**s1** | **str** | Форма единицы, используемая при числительном 1 | [optional] 
**s2** | **str** | Форма единицы, используемая при числительном 2 | [optional] 
**s5** | **str** | Форма единицы, используемая при числительном 5 | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.currency_minor_unit import CurrencyMinorUnit

# TODO update the JSON string below
json = "{}"
# create an instance of CurrencyMinorUnit from a JSON string
currency_minor_unit_instance = CurrencyMinorUnit.from_json(json)
# print the JSON string representation of the object
print(CurrencyMinorUnit.to_json())

# convert the object into a dict
currency_minor_unit_dict = currency_minor_unit_instance.to_dict()
# create an instance of CurrencyMinorUnit from a dict
currency_minor_unit_from_dict = CurrencyMinorUnit.from_dict(currency_minor_unit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


