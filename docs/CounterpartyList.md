# CounterpartyList

Список контрагентов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Counterparty]**](Counterparty.md) | Массив контрагентов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty_list import CounterpartyList

# TODO update the JSON string below
json = "{}"
# create an instance of CounterpartyList from a JSON string
counterparty_list_instance = CounterpartyList.from_json(json)
# print the JSON string representation of the object
print(CounterpartyList.to_json())

# convert the object into a dict
counterparty_list_dict = counterparty_list_instance.to_dict()
# create an instance of CounterpartyList from a dict
counterparty_list_from_dict = CounterpartyList.from_dict(counterparty_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


