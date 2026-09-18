# ReportTurnoverByStore

Строка отчета «Обороты по товару с детализацией по складам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment** | [**ReportTurnoverAssortment**](ReportTurnoverAssortment.md) |  | [optional] 
**stock_by_store** | [**List[ReportTurnoverByStoreItem]**](ReportTurnoverByStoreItem.md) | Детализация оборотов по складам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_by_store import ReportTurnoverByStore

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverByStore from a JSON string
report_turnover_by_store_instance = ReportTurnoverByStore.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverByStore.to_json())

# convert the object into a dict
report_turnover_by_store_dict = report_turnover_by_store_instance.to_dict()
# create an instance of ReportTurnoverByStore from a dict
report_turnover_by_store_from_dict = ReportTurnoverByStore.from_dict(report_turnover_by_store_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


