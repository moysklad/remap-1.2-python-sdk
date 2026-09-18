# StockCurrentByStore

Строка краткого отчета об остатках по складам. В ответе возвращается только одно поле значения остатка, выбранное параметром `stockType`. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment_id** | **str** | ID товара, модификации или партии | [optional] 
**store_id** | **str** | ID склада. Значение &#x60;null&#x60; может возвращаться для части резерва, не привязанной к складу.  | [optional] 
**stock** | **float** | Физический остаток на складах, без учета резерва и ожидания | [optional] 
**free_stock** | **float** | Остаток на складах за вычетом резерва | [optional] 
**quantity** | **float** | Доступно (учитывает резерв и ожидания) | [optional] 
**reserve** | **float** | Резерв | [optional] 
**in_transit** | **float** | Ожидание | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_current_by_store import StockCurrentByStore

# TODO update the JSON string below
json = "{}"
# create an instance of StockCurrentByStore from a JSON string
stock_current_by_store_instance = StockCurrentByStore.from_json(json)
# print the JSON string representation of the object
print(StockCurrentByStore.to_json())

# convert the object into a dict
stock_current_by_store_dict = stock_current_by_store_instance.to_dict()
# create an instance of StockCurrentByStore from a dict
stock_current_by_store_from_dict = StockCurrentByStore.from_dict(stock_current_by_store_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


