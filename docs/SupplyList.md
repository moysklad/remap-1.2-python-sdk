# SupplyList

Список Приемок

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Supply]**](Supply.md) | Массив Приемок | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.supply_list import SupplyList

# TODO update the JSON string below
json = "{}"
# create an instance of SupplyList from a JSON string
supply_list_instance = SupplyList.from_json(json)
# print the JSON string representation of the object
print(SupplyList.to_json())

# convert the object into a dict
supply_list_dict = supply_list_instance.to_dict()
# create an instance of SupplyList from a dict
supply_list_from_dict = SupplyList.from_dict(supply_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


