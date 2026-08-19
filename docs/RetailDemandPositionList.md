# RetailDemandPositionList

Список позиций Розничной продажи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[RetailDemandPosition]**](RetailDemandPosition.md) | Массив позиций Розничной продажи | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_demand_position_list import RetailDemandPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailDemandPositionList from a JSON string
retail_demand_position_list_instance = RetailDemandPositionList.from_json(json)
# print the JSON string representation of the object
print(RetailDemandPositionList.to_json())

# convert the object into a dict
retail_demand_position_list_dict = retail_demand_position_list_instance.to_dict()
# create an instance of RetailDemandPositionList from a dict
retail_demand_position_list_from_dict = RetailDemandPositionList.from_dict(retail_demand_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


