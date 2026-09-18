# ReportTurnoverIndicators

Показатели оборотов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sum** | **float** | Сумма себестоимости в копейках | [optional] 
**quantity** | **float** | Количество единиц товара | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_indicators import ReportTurnoverIndicators

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverIndicators from a JSON string
report_turnover_indicators_instance = ReportTurnoverIndicators.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverIndicators.to_json())

# convert the object into a dict
report_turnover_indicators_dict = report_turnover_indicators_instance.to_dict()
# create an instance of ReportTurnoverIndicators from a dict
report_turnover_indicators_from_dict = ReportTurnoverIndicators.from_dict(report_turnover_indicators_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


