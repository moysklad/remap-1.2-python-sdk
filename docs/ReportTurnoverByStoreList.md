# ReportTurnoverByStoreList

Отчет «Обороты по товару с детализацией по складам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportTurnoverByStore]**](ReportTurnoverByStore.md) | Массив строк отчета оборотов с детализацией по складам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_by_store_list import ReportTurnoverByStoreList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverByStoreList from a JSON string
report_turnover_by_store_list_instance = ReportTurnoverByStoreList.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverByStoreList.to_json())

# convert the object into a dict
report_turnover_by_store_list_dict = report_turnover_by_store_list_instance.to_dict()
# create an instance of ReportTurnoverByStoreList from a dict
report_turnover_by_store_list_from_dict = ReportTurnoverByStoreList.from_dict(report_turnover_by_store_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


