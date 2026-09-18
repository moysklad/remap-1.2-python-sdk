# CounterpartyAdjustmentList

Список Корректировок взаиморасчетов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CounterpartyAdjustment]**](CounterpartyAdjustment.md) | Массив Корректировок взаиморасчетов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty_adjustment_list import CounterpartyAdjustmentList

# TODO update the JSON string below
json = "{}"
# create an instance of CounterpartyAdjustmentList from a JSON string
counterparty_adjustment_list_instance = CounterpartyAdjustmentList.from_json(json)
# print the JSON string representation of the object
print(CounterpartyAdjustmentList.to_json())

# convert the object into a dict
counterparty_adjustment_list_dict = counterparty_adjustment_list_instance.to_dict()
# create an instance of CounterpartyAdjustmentList from a dict
counterparty_adjustment_list_from_dict = CounterpartyAdjustmentList.from_dict(counterparty_adjustment_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


