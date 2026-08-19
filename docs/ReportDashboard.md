# ReportDashboard

Показатели за день, неделю или месяц

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sales** | [**ReportDashboardPeriodMetrics**](ReportDashboardPeriodMetrics.md) |  | [optional] 
**orders** | [**ReportDashboardPeriodMetrics**](ReportDashboardPeriodMetrics.md) |  | [optional] 
**money** | [**ReportDashboardMoney**](ReportDashboardMoney.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_dashboard import ReportDashboard

# TODO update the JSON string below
json = "{}"
# create an instance of ReportDashboard from a JSON string
report_dashboard_instance = ReportDashboard.from_json(json)
# print the JSON string representation of the object
print(ReportDashboard.to_json())

# convert the object into a dict
report_dashboard_dict = report_dashboard_instance.to_dict()
# create an instance of ReportDashboard from a dict
report_dashboard_from_dict = ReportDashboard.from_dict(report_dashboard_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


