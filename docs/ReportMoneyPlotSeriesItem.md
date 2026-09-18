# ReportMoneyPlotSeriesItem

Показатель движения денежных средств за период отчета

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **str** | Дата показателя в формате YYYY-MM-DD HH:MM:SS | [optional] 
**credit** | **float** | Доход за период | [optional] 
**debit** | **float** | Расход за период | [optional] 
**balance** | **float** | Баланс (доход минус расход) | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_money_plot_series_item import ReportMoneyPlotSeriesItem

# TODO update the JSON string below
json = "{}"
# create an instance of ReportMoneyPlotSeriesItem from a JSON string
report_money_plot_series_item_instance = ReportMoneyPlotSeriesItem.from_json(json)
# print the JSON string representation of the object
print(ReportMoneyPlotSeriesItem.to_json())

# convert the object into a dict
report_money_plot_series_item_dict = report_money_plot_series_item_instance.to_dict()
# create an instance of ReportMoneyPlotSeriesItem from a dict
report_money_plot_series_item_from_dict = ReportMoneyPlotSeriesItem.from_dict(report_money_plot_series_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


