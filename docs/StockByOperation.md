# StockByOperation

Строка отчета «Остатки по документам».  `meta` — ссылка на документ, по которому выдаются остатки. Поддерживаемые типы документов: demand, customerorder, retaildemand, invoicein, invoiceout, purchaseorder, supply, retailsalesreturn, purchasereturn, salesreturn. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**positions** | [**List[StockByOperationPosition]**](StockByOperationPosition.md) | Массив остатков по каждой из позиций документа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_by_operation import StockByOperation

# TODO update the JSON string below
json = "{}"
# create an instance of StockByOperation from a JSON string
stock_by_operation_instance = StockByOperation.from_json(json)
# print the JSON string representation of the object
print(StockByOperation.to_json())

# convert the object into a dict
stock_by_operation_dict = stock_by_operation_instance.to_dict()
# create an instance of StockByOperation from a dict
stock_by_operation_from_dict = StockByOperation.from_dict(stock_by_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


