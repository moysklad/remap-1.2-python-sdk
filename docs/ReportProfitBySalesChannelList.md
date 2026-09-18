# ReportProfitBySalesChannelList

Отчет «Прибыльность по каналам продаж»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportProfitBySalesChannel]**](ReportProfitBySalesChannel.md) | Массив строк отчета прибыльности по каналам продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_by_sales_channel_list import ReportProfitBySalesChannelList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitBySalesChannelList from a JSON string
report_profit_by_sales_channel_list_instance = ReportProfitBySalesChannelList.from_json(json)
# print the JSON string representation of the object
print(ReportProfitBySalesChannelList.to_json())

# convert the object into a dict
report_profit_by_sales_channel_list_dict = report_profit_by_sales_channel_list_instance.to_dict()
# create an instance of ReportProfitBySalesChannelList from a dict
report_profit_by_sales_channel_list_from_dict = ReportProfitBySalesChannelList.from_dict(report_profit_by_sales_channel_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


