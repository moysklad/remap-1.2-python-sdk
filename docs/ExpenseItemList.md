# ExpenseItemList

Список статей расходов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ExpenseItem]**](ExpenseItem.md) | Массив статей расходов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.expense_item_list import ExpenseItemList

# TODO update the JSON string below
json = "{}"
# create an instance of ExpenseItemList from a JSON string
expense_item_list_instance = ExpenseItemList.from_json(json)
# print the JSON string representation of the object
print(ExpenseItemList.to_json())

# convert the object into a dict
expense_item_list_dict = expense_item_list_instance.to_dict()
# create an instance of ExpenseItemList from a dict
expense_item_list_from_dict = ExpenseItemList.from_dict(expense_item_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


