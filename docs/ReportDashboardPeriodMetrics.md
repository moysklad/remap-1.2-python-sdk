# ReportDashboardPeriodMetrics

Показатели продаж или заказов за период

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**count** | **int** | Количество продаж | [optional] 
**amount** | **int** | Прибыль | [optional] 
**movement_amount** | **int** | Дельта по сравнению с прошлым аналогичным периодом | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_dashboard_period_metrics import ReportDashboardPeriodMetrics

# TODO update the JSON string below
json = "{}"
# create an instance of ReportDashboardPeriodMetrics from a JSON string
report_dashboard_period_metrics_instance = ReportDashboardPeriodMetrics.from_json(json)
# print the JSON string representation of the object
print(ReportDashboardPeriodMetrics.to_json())

# convert the object into a dict
report_dashboard_period_metrics_dict = report_dashboard_period_metrics_instance.to_dict()
# create an instance of ReportDashboardPeriodMetrics from a dict
report_dashboard_period_metrics_from_dict = ReportDashboardPeriodMetrics.from_dict(report_dashboard_period_metrics_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


