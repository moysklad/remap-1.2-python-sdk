# RetailStoreList

Список точек продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[RetailStore]**](RetailStore.md) | Массив точек продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_list import RetailStoreList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreList from a JSON string
retail_store_list_instance = RetailStoreList.from_json(json)
# print the JSON string representation of the object
print(RetailStoreList.to_json())

# convert the object into a dict
retail_store_list_dict = retail_store_list_instance.to_dict()
# create an instance of RetailStoreList from a dict
retail_store_list_from_dict = RetailStoreList.from_dict(retail_store_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


