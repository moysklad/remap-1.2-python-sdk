# SalesReturnList

Список Возвратов покупателей

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[SalesReturn]**](SalesReturn.md) | Массив Возвратов покупателей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sales_return_list import SalesReturnList

# TODO update the JSON string below
json = "{}"
# create an instance of SalesReturnList from a JSON string
sales_return_list_instance = SalesReturnList.from_json(json)
# print the JSON string representation of the object
print(SalesReturnList.to_json())

# convert the object into a dict
sales_return_list_dict = sales_return_list_instance.to_dict()
# create an instance of SalesReturnList from a dict
sales_return_list_from_dict = SalesReturnList.from_dict(sales_return_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


