# FactureInList

Список Счетов-фактур полученных

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[FactureIn]**](FactureIn.md) | Массив Счетов-фактур полученных | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.facture_in_list import FactureInList

# TODO update the JSON string below
json = "{}"
# create an instance of FactureInList from a JSON string
facture_in_list_instance = FactureInList.from_json(json)
# print the JSON string representation of the object
print(FactureInList.to_json())

# convert the object into a dict
facture_in_list_dict = facture_in_list_instance.to_dict()
# create an instance of FactureInList from a dict
facture_in_list_from_dict = FactureInList.from_dict(facture_in_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


