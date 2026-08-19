# CashInList

Список Приходных ордеров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CashIn]**](CashIn.md) | Массив Приходных ордеров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.cash_in_list import CashInList

# TODO update the JSON string below
json = "{}"
# create an instance of CashInList from a JSON string
cash_in_list_instance = CashInList.from_json(json)
# print the JSON string representation of the object
print(CashInList.to_json())

# convert the object into a dict
cash_in_list_dict = cash_in_list_instance.to_dict()
# create an instance of CashInList from a dict
cash_in_list_from_dict = CashInList.from_dict(cash_in_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


