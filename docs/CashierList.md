# CashierList

Список кассиров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Cashier]**](Cashier.md) | Массив кассиров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.cashier_list import CashierList

# TODO update the JSON string below
json = "{}"
# create an instance of CashierList from a JSON string
cashier_list_instance = CashierList.from_json(json)
# print the JSON string representation of the object
print(CashierList.to_json())

# convert the object into a dict
cashier_list_dict = cashier_list_instance.to_dict()
# create an instance of CashierList from a dict
cashier_list_from_dict = CashierList.from_dict(cashier_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


