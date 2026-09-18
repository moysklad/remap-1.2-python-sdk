# ReportCounterpartyQueryCounterpartiesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**counterparty** | [**Counterparty**](Counterparty.md) | Контрагент, по которому требуется отчет | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_counterparty_query_counterparties_inner import ReportCounterpartyQueryCounterpartiesInner

# TODO update the JSON string below
json = "{}"
# create an instance of ReportCounterpartyQueryCounterpartiesInner from a JSON string
report_counterparty_query_counterparties_inner_instance = ReportCounterpartyQueryCounterpartiesInner.from_json(json)
# print the JSON string representation of the object
print(ReportCounterpartyQueryCounterpartiesInner.to_json())

# convert the object into a dict
report_counterparty_query_counterparties_inner_dict = report_counterparty_query_counterparties_inner_instance.to_dict()
# create an instance of ReportCounterpartyQueryCounterpartiesInner from a dict
report_counterparty_query_counterparties_inner_from_dict = ReportCounterpartyQueryCounterpartiesInner.from_dict(report_counterparty_query_counterparties_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


