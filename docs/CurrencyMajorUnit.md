# CurrencyMajorUnit

Формы единиц целой части Валюты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**gender** | **str** | Пол. Известные значения описаны в Gender | [optional] 
**s1** | **str** | Форма единицы, используемая при числительном 1 | [optional] 
**s2** | **str** | Форма единицы, используемая при числительном 2 | [optional] 
**s5** | **str** | Форма единицы, используемая при числительном 5 | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.currency_major_unit import CurrencyMajorUnit

# TODO update the JSON string below
json = "{}"
# create an instance of CurrencyMajorUnit from a JSON string
currency_major_unit_instance = CurrencyMajorUnit.from_json(json)
# print the JSON string representation of the object
print(CurrencyMajorUnit.to_json())

# convert the object into a dict
currency_major_unit_dict = currency_major_unit_instance.to_dict()
# create an instance of CurrencyMajorUnit from a dict
currency_major_unit_from_dict = CurrencyMajorUnit.from_dict(currency_major_unit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


