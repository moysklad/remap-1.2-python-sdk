# ReportTurnover

Строка отчета «Обороты по товарам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment** | [**ReportTurnoverAssortment**](ReportTurnoverAssortment.md) |  | [optional] 
**on_period_start** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 
**on_period_end** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 
**income** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 
**outcome** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover import ReportTurnover

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnover from a JSON string
report_turnover_instance = ReportTurnover.from_json(json)
# print the JSON string representation of the object
print(ReportTurnover.to_json())

# convert the object into a dict
report_turnover_dict = report_turnover_instance.to_dict()
# create an instance of ReportTurnover from a dict
report_turnover_from_dict = ReportTurnover.from_dict(report_turnover_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


