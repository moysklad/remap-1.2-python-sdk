# ReportCounterparty

Строка отчета «Показатели контрагентов»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**counterparty** | [**Counterparty**](Counterparty.md) |  | [optional] 
**first_demand_date** | **str** | Дата первой продажи | [optional] 
**last_demand_date** | **str** | Дата последней продажи | [optional] 
**demands_count** | **int** | Количество продаж | [optional] 
**demands_sum** | **float** | Сумма продаж | [optional] 
**average_receipt** | **float** | Средний чек | [optional] 
**returns_count** | **int** | Количество возвратов | [optional] 
**returns_sum** | **float** | Сумма возвратов | [optional] 
**discounts_sum** | **float** | Сумма скидок | [optional] 
**balance** | **float** | Баланс | [optional] 
**bonus_balance** | **float** | Баллы | [optional] 
**profit** | **float** | Прибыль | [optional] 
**last_event_date** | **str** | Дата последнего события | [optional] 
**last_event_text** | **str** | Текст последнего события | [optional] 
**updated** | **str** | Момент последнего изменения контрагента | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_counterparty import ReportCounterparty

# TODO update the JSON string below
json = "{}"
# create an instance of ReportCounterparty from a JSON string
report_counterparty_instance = ReportCounterparty.from_json(json)
# print the JSON string representation of the object
print(ReportCounterparty.to_json())

# convert the object into a dict
report_counterparty_dict = report_counterparty_instance.to_dict()
# create an instance of ReportCounterparty from a dict
report_counterparty_from_dict = ReportCounterparty.from_dict(report_counterparty_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


