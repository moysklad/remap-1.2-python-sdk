# StockAll

Строка Расширенного отчета об остатках.  Тип каждой строки задается её `meta.type` (product, variant или consignment). Параметр запроса `groupBy` определяет набор возможных типов в выдаче: `product` — только товары; `variant` — товары и модификации; `consignment` — товары, модификации и партии. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**name** | **str** | Наименование | [optional] 
**code** | **str** | Код | [optional] 
**article** | **str** | Артикул | [optional] 
**external_code** | **str** | Внешний код сущности, по которой выводится остаток | [optional] 
**folder** | [**ProductFolder**](ProductFolder.md) |  | [optional] 
**image** | [**Image**](Image.md) |  | [optional] 
**uom** | [**Uom**](Uom.md) |  | [optional] 
**stock** | **float** | Остаток | [optional] 
**in_transit** | **float** | Ожидание | [optional] 
**reserve** | **float** | Резерв | [optional] 
**quantity** | **float** | Доступно | [optional] 
**stock_days** | **int** | Количество дней на складе | [optional] 
**price** | **float** | Себестоимость в копейках | [optional] 
**sale_price** | **float** | Цена продажи | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.stock_all import StockAll

# TODO update the JSON string below
json = "{}"
# create an instance of StockAll from a JSON string
stock_all_instance = StockAll.from_json(json)
# print the JSON string representation of the object
print(StockAll.to_json())

# convert the object into a dict
stock_all_dict = stock_all_instance.to_dict()
# create an instance of StockAll from a dict
stock_all_from_dict = StockAll.from_dict(stock_all_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


