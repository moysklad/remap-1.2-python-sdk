# ReportProfitByVariant

Строка отчета «Прибыльность по модификациям»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment** | [**ReportProfitAssortment**](ReportProfitAssortment.md) |  | [optional] 
**margin** | **float** | Рентабельность товара | [optional] 
**sales_margin** | **float** | Рентабельность продаж | [optional] 
**profit** | **float** | Прибыль | [optional] 
**return_cost** | **float** | Себестоимость возвратов в копейках | [optional] 
**return_cost_sum** | **float** | Сумма себестоимостей возвратов в копейках | [optional] 
**return_price** | **float** | Цена возвратов | [optional] 
**return_quantity** | **float** | Возвращенное количество | [optional] 
**return_sum** | **float** | Сумма возвратов | [optional] 
**sell_cost** | **float** | Себестоимость в копейках | [optional] 
**sell_cost_sum** | **float** | Сумма себестоимостей продаж в копейках | [optional] 
**sell_price** | **float** | Средняя цена продаж | [optional] 
**sell_quantity** | **float** | Проданное количество | [optional] 
**sell_sum** | **float** | Сумма продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_by_variant import ReportProfitByVariant

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitByVariant from a JSON string
report_profit_by_variant_instance = ReportProfitByVariant.from_json(json)
# print the JSON string representation of the object
print(ReportProfitByVariant.to_json())

# convert the object into a dict
report_profit_by_variant_dict = report_profit_by_variant_instance.to_dict()
# create an instance of ReportProfitByVariant from a dict
report_profit_by_variant_from_dict = ReportProfitByVariant.from_dict(report_profit_by_variant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


