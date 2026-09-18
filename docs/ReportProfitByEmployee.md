# ReportProfitByEmployee

Строка отчета «Прибыльность по сотрудникам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee** | [**Employee**](Employee.md) |  | [optional] 
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
from moysklad_remap_12_sdk.models.report_profit_by_employee import ReportProfitByEmployee

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitByEmployee from a JSON string
report_profit_by_employee_instance = ReportProfitByEmployee.from_json(json)
# print the JSON string representation of the object
print(ReportProfitByEmployee.to_json())

# convert the object into a dict
report_profit_by_employee_dict = report_profit_by_employee_instance.to_dict()
# create an instance of ReportProfitByEmployee from a dict
report_profit_by_employee_from_dict = ReportProfitByEmployee.from_dict(report_profit_by_employee_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


