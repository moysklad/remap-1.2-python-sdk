# ReportMoneyPlotSeries

Отчет о движении денежных средств

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**credit** | **float** | Доход за весь период отчета | [optional] 
**debit** | **float** | Расход за весь период отчета | [optional] 
**series** | [**List[ReportMoneyPlotSeriesItem]**](ReportMoneyPlotSeriesItem.md) | Массив показателей движения денежных средств | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_money_plot_series import ReportMoneyPlotSeries

# TODO update the JSON string below
json = "{}"
# create an instance of ReportMoneyPlotSeries from a JSON string
report_money_plot_series_instance = ReportMoneyPlotSeries.from_json(json)
# print the JSON string representation of the object
print(ReportMoneyPlotSeries.to_json())

# convert the object into a dict
report_money_plot_series_dict = report_money_plot_series_instance.to_dict()
# create an instance of ReportMoneyPlotSeries from a dict
report_money_plot_series_from_dict = ReportMoneyPlotSeries.from_dict(report_money_plot_series_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


