# ReportDashboardMoney

Информация о деньгах за период

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**income** | **int** | Доходы за период | [optional] 
**outcome** | **float** | Расходы за период | [optional] 
**balance** | **float** | Текущий баланс | [optional] 
**today_movement** | **float** | Дельта за сегодня | [optional] 
**movement** | **float** | Дельта за период | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_dashboard_money import ReportDashboardMoney

# TODO update the JSON string below
json = "{}"
# create an instance of ReportDashboardMoney from a JSON string
report_dashboard_money_instance = ReportDashboardMoney.from_json(json)
# print the JSON string representation of the object
print(ReportDashboardMoney.to_json())

# convert the object into a dict
report_dashboard_money_dict = report_dashboard_money_instance.to_dict()
# create an instance of ReportDashboardMoney from a dict
report_dashboard_money_from_dict = ReportDashboardMoney.from_dict(report_dashboard_money_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


