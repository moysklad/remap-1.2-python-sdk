# BonusTransactionList

Список бонусных операций

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[BonusTransaction]**](BonusTransaction.md) | Массив бонусных операций | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bonus_transaction_list import BonusTransactionList

# TODO update the JSON string below
json = "{}"
# create an instance of BonusTransactionList from a JSON string
bonus_transaction_list_instance = BonusTransactionList.from_json(json)
# print the JSON string representation of the object
print(BonusTransactionList.to_json())

# convert the object into a dict
bonus_transaction_list_dict = bonus_transaction_list_instance.to_dict()
# create an instance of BonusTransactionList from a dict
bonus_transaction_list_from_dict = BonusTransactionList.from_dict(bonus_transaction_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


