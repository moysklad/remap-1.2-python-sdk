# ReportOrdersPlotSeriesList

Показатели заказов покупателей

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**series** | [**List[ReportPlotSeries]**](ReportPlotSeries.md) | Массив показателей заказов | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_orders_plot_series_list import ReportOrdersPlotSeriesList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportOrdersPlotSeriesList from a JSON string
report_orders_plot_series_list_instance = ReportOrdersPlotSeriesList.from_json(json)
# print the JSON string representation of the object
print(ReportOrdersPlotSeriesList.to_json())

# convert the object into a dict
report_orders_plot_series_list_dict = report_orders_plot_series_list_instance.to_dict()
# create an instance of ReportOrdersPlotSeriesList from a dict
report_orders_plot_series_list_from_dict = ReportOrdersPlotSeriesList.from_dict(report_orders_plot_series_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


