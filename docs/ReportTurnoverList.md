# ReportTurnoverList

Отчет «Обороты по товарам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportTurnover]**](ReportTurnover.md) | Массив строк отчета оборотов по товарам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_list import ReportTurnoverList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverList from a JSON string
report_turnover_list_instance = ReportTurnoverList.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverList.to_json())

# convert the object into a dict
report_turnover_list_dict = report_turnover_list_instance.to_dict()
# create an instance of ReportTurnoverList from a dict
report_turnover_list_from_dict = ReportTurnoverList.from_dict(report_turnover_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


