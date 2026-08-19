# SalesChannelList

Список Каналов продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[SalesChannel]**](SalesChannel.md) | Массив Каналов продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sales_channel_list import SalesChannelList

# TODO update the JSON string below
json = "{}"
# create an instance of SalesChannelList from a JSON string
sales_channel_list_instance = SalesChannelList.from_json(json)
# print the JSON string representation of the object
print(SalesChannelList.to_json())

# convert the object into a dict
sales_channel_list_dict = sales_channel_list_instance.to_dict()
# create an instance of SalesChannelList from a dict
sales_channel_list_from_dict = SalesChannelList.from_dict(sales_channel_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


