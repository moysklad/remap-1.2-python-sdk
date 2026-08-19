# FactureOutList

Список Счетов-фактур выданных

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[FactureOut]**](FactureOut.md) | Массив Счетов-фактур выданных | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.facture_out_list import FactureOutList

# TODO update the JSON string below
json = "{}"
# create an instance of FactureOutList from a JSON string
facture_out_list_instance = FactureOutList.from_json(json)
# print the JSON string representation of the object
print(FactureOutList.to_json())

# convert the object into a dict
facture_out_list_dict = facture_out_list_instance.to_dict()
# create an instance of FactureOutList from a dict
facture_out_list_from_dict = FactureOutList.from_dict(facture_out_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


