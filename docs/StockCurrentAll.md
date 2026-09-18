# StockCurrentAll

Строка краткого отчета об остатках по всей номенклатуре. В ответе возвращается только одно поле значения остатка, выбранное параметром `stockType`. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment_id** | **str** | ID товара, модификации или партии | [optional] 
**stock** | **float** | Физический остаток на складах, без учета резерва и ожидания | [optional] 
**free_stock** | **float** | Остаток на складах за вычетом резерва | [optional] 
**quantity** | **float** | Доступно (учитывает резерв и ожидания) | [optional] 
**reserve** | **float** | Резерв | [optional] 
**in_transit** | **float** | Ожидание | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_current_all import StockCurrentAll

# TODO update the JSON string below
json = "{}"
# create an instance of StockCurrentAll from a JSON string
stock_current_all_instance = StockCurrentAll.from_json(json)
# print the JSON string representation of the object
print(StockCurrentAll.to_json())

# convert the object into a dict
stock_current_all_dict = stock_current_all_instance.to_dict()
# create an instance of StockCurrentAll from a dict
stock_current_all_from_dict = StockCurrentAll.from_dict(stock_current_all_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


