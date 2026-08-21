# ByOperationsStock

Строка отчета по документам номенклатуры, отображающего остатки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment** | [**ByOperationsStockAssortment**](ByOperationsStockAssortment.md) |  | [optional] 
**operation** | [**ByOperationsStockOperation**](ByOperationsStockOperation.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**store** | [**ByOperationsStockStore**](ByOperationsStockStore.md) |  | [optional] 
**stock** | **float** | Остатки | [optional] 
**cost_per_unit** | **float** | Себестоимость за единицу. Не возвращается при отсутствии пермиссии «Видеть себестоимость, цену закупки, прибыль товаров».  | [optional] 
**sum_cost** | **float** | Сумма себестоимости. Не возвращается при отсутствии пермиссии «Видеть себестоимость, цену закупки, прибыль товаров».  | [optional] 
**avg_stock_days** | **float** | Количество дней на складе | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.by_operations_stock import ByOperationsStock

# TODO update the JSON string below
json = "{}"
# create an instance of ByOperationsStock from a JSON string
by_operations_stock_instance = ByOperationsStock.from_json(json)
# print the JSON string representation of the object
print(ByOperationsStock.to_json())

# convert the object into a dict
by_operations_stock_dict = by_operations_stock_instance.to_dict()
# create an instance of ByOperationsStock from a dict
by_operations_stock_from_dict = ByOperationsStock.from_dict(by_operations_stock_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


