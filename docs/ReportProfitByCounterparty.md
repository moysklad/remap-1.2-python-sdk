# ReportProfitByCounterparty

Строка отчета «Прибыльность по покупателям»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**counterparty** | [**Counterparty**](Counterparty.md) |  | [optional] 
**margin** | **float** | Рентабельность | [optional] 
**sales_margin** | **float** | Рентабельность продаж | [optional] 
**profit** | **float** | Прибыль | [optional] 
**return_avg_check** | **float** | Средний чек возврата | [optional] 
**return_cost_sum** | **float** | Сумма себестоимостей возвратов в копейках | [optional] 
**return_count** | **int** | Количество возвратов | [optional] 
**return_sum** | **float** | Сумма возвратов | [optional] 
**sales_avg_check** | **float** | Средний чек продаж | [optional] 
**sales_count** | **int** | Количество продаж | [optional] 
**sell_cost_sum** | **float** | Сумма себестоимостей продаж в копейках | [optional] 
**sell_sum** | **float** | Сумма продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_by_counterparty import ReportProfitByCounterparty

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitByCounterparty from a JSON string
report_profit_by_counterparty_instance = ReportProfitByCounterparty.from_json(json)
# print the JSON string representation of the object
print(ReportProfitByCounterparty.to_json())

# convert the object into a dict
report_profit_by_counterparty_dict = report_profit_by_counterparty_instance.to_dict()
# create an instance of ReportProfitByCounterparty from a dict
report_profit_by_counterparty_from_dict = ReportProfitByCounterparty.from_dict(report_profit_by_counterparty_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


