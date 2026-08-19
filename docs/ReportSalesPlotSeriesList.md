# ReportSalesPlotSeriesList

Показатели продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**series** | [**List[ReportPlotSeries]**](ReportPlotSeries.md) | Массив показателей продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_sales_plot_series_list import ReportSalesPlotSeriesList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportSalesPlotSeriesList from a JSON string
report_sales_plot_series_list_instance = ReportSalesPlotSeriesList.from_json(json)
# print the JSON string representation of the object
print(ReportSalesPlotSeriesList.to_json())

# convert the object into a dict
report_sales_plot_series_list_dict = report_sales_plot_series_list_instance.to_dict()
# create an instance of ReportSalesPlotSeriesList from a dict
report_sales_plot_series_list_from_dict = ReportSalesPlotSeriesList.from_dict(report_sales_plot_series_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


