# ReportTurnoverByStoreItem

Детализация оборотов по одному складу

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**store** | [**Store**](Store.md) |  | [optional] 
**on_period_start** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 
**on_period_end** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 
**income** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 
**outcome** | [**ReportTurnoverIndicators**](ReportTurnoverIndicators.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_by_store_item import ReportTurnoverByStoreItem

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverByStoreItem from a JSON string
report_turnover_by_store_item_instance = ReportTurnoverByStoreItem.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverByStoreItem.to_json())

# convert the object into a dict
report_turnover_by_store_item_dict = report_turnover_by_store_item_instance.to_dict()
# create an instance of ReportTurnoverByStoreItem from a dict
report_turnover_by_store_item_from_dict = ReportTurnoverByStoreItem.from_dict(report_turnover_by_store_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


