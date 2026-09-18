# ReportCounterpartyList

Отчет «Показатели контрагентов»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportCounterparty]**](ReportCounterparty.md) | Массив JSON объектов, представляющих отчеты по отдельным контрагентам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_counterparty_list import ReportCounterpartyList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportCounterpartyList from a JSON string
report_counterparty_list_instance = ReportCounterpartyList.from_json(json)
# print the JSON string representation of the object
print(ReportCounterpartyList.to_json())

# convert the object into a dict
report_counterparty_list_dict = report_counterparty_list_instance.to_dict()
# create an instance of ReportCounterpartyList from a dict
report_counterparty_list_from_dict = ReportCounterpartyList.from_dict(report_counterparty_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


