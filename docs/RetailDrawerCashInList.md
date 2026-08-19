# RetailDrawerCashInList

Список Внесений денег

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[RetailDrawerCashIn]**](RetailDrawerCashIn.md) | Массив Внесений денег | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_drawer_cash_in_list import RetailDrawerCashInList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDrawerCashInList from a JSON string
retail_drawer_cash_in_list_instance = RetailDrawerCashInList.from_json(json)
# print the JSON string representation of the object
print(RetailDrawerCashInList.to_json())

# convert the object into a dict
retail_drawer_cash_in_list_dict = retail_drawer_cash_in_list_instance.to_dict()
# create an instance of RetailDrawerCashInList from a dict
retail_drawer_cash_in_list_from_dict = RetailDrawerCashInList.from_dict(retail_drawer_cash_in_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


