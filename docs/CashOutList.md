# CashOutList

Список Расходных ордеров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CashOut]**](CashOut.md) | Массив Расходных ордеров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.cash_out_list import CashOutList

# TODO update the JSON string below
json = "{}"
# create an instance of CashOutList from a JSON string
cash_out_list_instance = CashOutList.from_json(json)
# print the JSON string representation of the object
print(CashOutList.to_json())

# convert the object into a dict
cash_out_list_dict = cash_out_list_instance.to_dict()
# create an instance of CashOutList from a dict
cash_out_list_from_dict = CashOutList.from_dict(cash_out_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


