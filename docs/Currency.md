# Currency

Валюта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID валюты | [optional] [readonly] 
**system** | **bool** | Системная валюта | [optional] 
**name** | **str** | Краткое наименование валюты | [optional] 
**full_name** | **str** | Полное наименование валюты | [optional] 
**code** | **str** | Цифровой код валюты | [optional] 
**iso_code** | **str** | Буквенный код валюты | [optional] 
**multiplicity** | **int** | Кратность курса валюты | [optional] 
**rate** | **float** | Курс валюты | [optional] 
**margin** | **float** | Наценка при автоматическом обновлении курса | [optional] 
**indirect** | **bool** | Признак обратного курса валюты | [optional] 
**rate_update_type** | **str** | Способ обновления курса валюты. Известные значения описаны в RateUpdateType | [optional] 
**archived** | **bool** | Добавлена ли валюта в архив | [optional] 
**default** | **bool** | Валюта учета по умолчанию | [optional] 
**major_unit** | [**CurrencyMajorUnit**](CurrencyMajorUnit.md) |  | [optional] 
**minor_unit** | [**CurrencyMinorUnit**](CurrencyMinorUnit.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.currency import Currency

# TODO update the JSON string below
json = "{}"
# create an instance of Currency from a JSON string
currency_instance = Currency.from_json(json)
# print the JSON string representation of the object
print(Currency.to_json())

# convert the object into a dict
currency_dict = currency_instance.to_dict()
# create an instance of Currency from a dict
currency_from_dict = Currency.from_dict(currency_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


