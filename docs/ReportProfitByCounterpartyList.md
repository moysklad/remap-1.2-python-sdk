# ReportProfitByCounterpartyList

Отчет «Прибыльность по покупателям»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportProfitByCounterparty]**](ReportProfitByCounterparty.md) | Массив строк отчета прибыльности по покупателям | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_by_counterparty_list import ReportProfitByCounterpartyList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitByCounterpartyList from a JSON string
report_profit_by_counterparty_list_instance = ReportProfitByCounterpartyList.from_json(json)
# print the JSON string representation of the object
print(ReportProfitByCounterpartyList.to_json())

# convert the object into a dict
report_profit_by_counterparty_list_dict = report_profit_by_counterparty_list_instance.to_dict()
# create an instance of ReportProfitByCounterpartyList from a dict
report_profit_by_counterparty_list_from_dict = ReportProfitByCounterpartyList.from_dict(report_profit_by_counterparty_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


