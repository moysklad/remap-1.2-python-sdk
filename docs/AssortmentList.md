# AssortmentList

Список ассортимента

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Assortment]**](Assortment.md) | Массив элементов ассортимента | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.assortment_list import AssortmentList

# TODO update the JSON string below
json = "{}"
# create an instance of AssortmentList from a JSON string
assortment_list_instance = AssortmentList.from_json(json)
# print the JSON string representation of the object
print(AssortmentList.to_json())

# convert the object into a dict
assortment_list_dict = assortment_list_instance.to_dict()
# create an instance of AssortmentList from a dict
assortment_list_from_dict = AssortmentList.from_dict(assortment_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


