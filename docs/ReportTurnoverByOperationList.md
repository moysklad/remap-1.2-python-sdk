# ReportTurnoverByOperationList

Отчет «Обороты по товару с детализацией по документам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportTurnoverByOperation]**](ReportTurnoverByOperation.md) | Массив строк отчета оборотов с детализацией по документам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_by_operation_list import ReportTurnoverByOperationList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverByOperationList from a JSON string
report_turnover_by_operation_list_instance = ReportTurnoverByOperationList.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverByOperationList.to_json())

# convert the object into a dict
report_turnover_by_operation_list_dict = report_turnover_by_operation_list_instance.to_dict()
# create an instance of ReportTurnoverByOperationList from a dict
report_turnover_by_operation_list_from_dict = ReportTurnoverByOperationList.from_dict(report_turnover_by_operation_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


