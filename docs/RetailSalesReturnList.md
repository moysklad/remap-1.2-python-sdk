# RetailSalesReturnList

Список Розничных возвратов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[RetailSalesReturn]**](RetailSalesReturn.md) | Массив Розничных возвратов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_sales_return_list import RetailSalesReturnList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailSalesReturnList from a JSON string
retail_sales_return_list_instance = RetailSalesReturnList.from_json(json)
# print the JSON string representation of the object
print(RetailSalesReturnList.to_json())

# convert the object into a dict
retail_sales_return_list_dict = retail_sales_return_list_instance.to_dict()
# create an instance of RetailSalesReturnList from a dict
retail_sales_return_list_from_dict = RetailSalesReturnList.from_dict(retail_sales_return_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


