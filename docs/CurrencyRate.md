# CurrencyRate

Валюта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | [**Currency**](.md) | Валюта | [optional] 
**value** | **float** | Курс валюты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.currency_rate import CurrencyRate

# TODO update the JSON string below
json = "{}"
# create an instance of CurrencyRate from a JSON string
currency_rate_instance = CurrencyRate.from_json(json)
# print the JSON string representation of the object
print(CurrencyRate.to_json())

# convert the object into a dict
currency_rate_dict = currency_rate_instance.to_dict()
# create an instance of CurrencyRate from a dict
currency_rate_from_dict = CurrencyRate.from_dict(currency_rate_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


