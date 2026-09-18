# ReportTurnoverOperation

Документ, связанный с Товаром

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**name** | **str** | Номер документа | [optional] 
**description** | **str** | Комментарий к документу | [optional] 
**moment** | **str** | Дата проведения документа | [optional] 
**agent** | [**Agent**](Agent.md) | Контрагент документа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_operation import ReportTurnoverOperation

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverOperation from a JSON string
report_turnover_operation_instance = ReportTurnoverOperation.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverOperation.to_json())

# convert the object into a dict
report_turnover_operation_dict = report_turnover_operation_instance.to_dict()
# create an instance of ReportTurnoverOperation from a dict
report_turnover_operation_from_dict = ReportTurnoverOperation.from_dict(report_turnover_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


