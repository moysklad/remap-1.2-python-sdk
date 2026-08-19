# TaxRateList

Список ставок НДС

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[TaxRate]**](TaxRate.md) | Массив ставок НДС | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.tax_rate_list import TaxRateList

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRateList from a JSON string
tax_rate_list_instance = TaxRateList.from_json(json)
# print the JSON string representation of the object
print(TaxRateList.to_json())

# convert the object into a dict
tax_rate_list_dict = tax_rate_list_instance.to_dict()
# create an instance of TaxRateList from a dict
tax_rate_list_from_dict = TaxRateList.from_dict(tax_rate_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


