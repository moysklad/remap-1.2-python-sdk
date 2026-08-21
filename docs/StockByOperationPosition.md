# StockByOperationPosition

Остаток по позиции в отчете «Остатки по документам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**name** | **str** | Наименование позиции | [optional] 
**stock** | **float** | Остаток | [optional] 
**cost** | **float** | Себестоимость в копейках | [optional] 
**in_transit** | **float** | Ожидание. У сущности Комплект значение всегда &#x60;0&#x60; | [optional] 
**reserve** | **float** | Резерв. У сущности Комплект значение всегда &#x60;0&#x60; | [optional] 
**quantity** | **float** | Доступно. У сущности Комплект значение всегда &#x60;0&#x60; | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_by_operation_position import StockByOperationPosition

# TODO update the JSON string below
json = "{}"
# create an instance of StockByOperationPosition from a JSON string
stock_by_operation_position_instance = StockByOperationPosition.from_json(json)
# print the JSON string representation of the object
print(StockByOperationPosition.to_json())

# convert the object into a dict
stock_by_operation_position_dict = stock_by_operation_position_instance.to_dict()
# create an instance of StockByOperationPosition from a dict
stock_by_operation_position_from_dict = StockByOperationPosition.from_dict(stock_by_operation_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


