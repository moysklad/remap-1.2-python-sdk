# RetailDemandList

Список Розничных продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[RetailDemand]**](RetailDemand.md) | Массив Розничных продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_demand_list import RetailDemandList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDemandList from a JSON string
retail_demand_list_instance = RetailDemandList.from_json(json)
# print the JSON string representation of the object
print(RetailDemandList.to_json())

# convert the object into a dict
retail_demand_list_dict = retail_demand_list_instance.to_dict()
# create an instance of RetailDemandList from a dict
retail_demand_list_from_dict = RetailDemandList.from_dict(retail_demand_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


