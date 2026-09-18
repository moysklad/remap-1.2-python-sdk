# ReportCounterpartyQuery

Запрос выборочных показателей контрагентов

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**counterparties** | [**List[ReportCounterpartyQueryCounterpartiesInner]**](ReportCounterpartyQueryCounterpartiesInner.md) | Массив контрагентов, по которым требуются отчеты | 

## Example

```python
from moysklad_remap_12_sdk.models.report_counterparty_query import ReportCounterpartyQuery

# TODO update the JSON string below
json = "{}"
# create an instance of ReportCounterpartyQuery from a JSON string
report_counterparty_query_instance = ReportCounterpartyQuery.from_json(json)
# print the JSON string representation of the object
print(ReportCounterpartyQuery.to_json())

# convert the object into a dict
report_counterparty_query_dict = report_counterparty_query_instance.to_dict()
# create an instance of ReportCounterpartyQuery from a dict
report_counterparty_query_from_dict = ReportCounterpartyQuery.from_dict(report_counterparty_query_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


