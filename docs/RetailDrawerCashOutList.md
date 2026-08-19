# RetailDrawerCashOutList

Список Выплат денег

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[RetailDrawerCashOut]**](RetailDrawerCashOut.md) | Массив Выплат денег | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_drawer_cash_out_list import RetailDrawerCashOutList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDrawerCashOutList from a JSON string
retail_drawer_cash_out_list_instance = RetailDrawerCashOutList.from_json(json)
# print the JSON string representation of the object
print(RetailDrawerCashOutList.to_json())

# convert the object into a dict
retail_drawer_cash_out_list_dict = retail_drawer_cash_out_list_instance.to_dict()
# create an instance of RetailDrawerCashOutList from a dict
retail_drawer_cash_out_list_from_dict = RetailDrawerCashOutList.from_dict(retail_drawer_cash_out_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


