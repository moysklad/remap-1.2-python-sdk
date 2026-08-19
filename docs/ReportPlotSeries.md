# ReportPlotSeries

Показатель продаж или заказов за период отчета

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **str** | Дата показателя в формате YYYY-MM-DD HH:MM:SS | [optional] 
**quantity** | **int** | Количество | [optional] 
**sum** | **float** | Сумма | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_plot_series import ReportPlotSeries

# TODO update the JSON string below
json = "{}"
# create an instance of ReportPlotSeries from a JSON string
report_plot_series_instance = ReportPlotSeries.from_json(json)
# print the JSON string representation of the object
print(ReportPlotSeries.to_json())

# convert the object into a dict
report_plot_series_dict = report_plot_series_instance.to_dict()
# create an instance of ReportPlotSeries from a dict
report_plot_series_from_dict = ReportPlotSeries.from_dict(report_plot_series_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


