# StoreBalanceList

Неснижаемые остатки по складам

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[StoreBalance]**](StoreBalance.md) | Массив элементов списка | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store_balance_list import StoreBalanceList

# TODO update the JSON string below
json = "{}"
# create an instance of StoreBalanceList from a JSON string
store_balance_list_instance = StoreBalanceList.from_json(json)
# print the JSON string representation of the object
print(StoreBalanceList.to_json())

# convert the object into a dict
store_balance_list_dict = store_balance_list_instance.to_dict()
# create an instance of StoreBalanceList from a dict
store_balance_list_from_dict = StoreBalanceList.from_dict(store_balance_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


