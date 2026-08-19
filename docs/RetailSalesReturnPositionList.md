# RetailSalesReturnPositionList

Список позиций Розничного возврата

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[RetailSalesReturnPosition]**](RetailSalesReturnPosition.md) | Массив позиций Розничного возврата | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_sales_return_position_list import RetailSalesReturnPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailSalesReturnPositionList from a JSON string
retail_sales_return_position_list_instance = RetailSalesReturnPositionList.from_json(json)
# print the JSON string representation of the object
print(RetailSalesReturnPositionList.to_json())

# convert the object into a dict
retail_sales_return_position_list_dict = retail_sales_return_position_list_instance.to_dict()
# create an instance of RetailSalesReturnPositionList from a dict
retail_sales_return_position_list_from_dict = RetailSalesReturnPositionList.from_dict(retail_sales_return_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


