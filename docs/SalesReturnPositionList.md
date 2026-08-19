# SalesReturnPositionList

Список позиций Возврата покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[SalesReturnPosition]**](SalesReturnPosition.md) | Массив позиций Возврата покупателя | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sales_return_position_list import SalesReturnPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of SalesReturnPositionList from a JSON string
sales_return_position_list_instance = SalesReturnPositionList.from_json(json)
# print the JSON string representation of the object
print(SalesReturnPositionList.to_json())

# convert the object into a dict
sales_return_position_list_dict = sales_return_position_list_instance.to_dict()
# create an instance of SalesReturnPositionList from a dict
sales_return_position_list_from_dict = SalesReturnPositionList.from_dict(sales_return_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


