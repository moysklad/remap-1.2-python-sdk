# RetailStoreLastOperationNamesInner

Последние операции

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**entity** | **str** | Ключевое слово, обозначающее тип последней операции | [optional] 
**name** | **str** | Наименование (номер) последней операции | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_last_operation_names_inner import RetailStoreLastOperationNamesInner

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreLastOperationNamesInner from a JSON string
retail_store_last_operation_names_inner_instance = RetailStoreLastOperationNamesInner.from_json(json)
# print the JSON string representation of the object
print(RetailStoreLastOperationNamesInner.to_json())

# convert the object into a dict
retail_store_last_operation_names_inner_dict = retail_store_last_operation_names_inner_instance.to_dict()
# create an instance of RetailStoreLastOperationNamesInner from a dict
retail_store_last_operation_names_inner_from_dict = RetailStoreLastOperationNamesInner.from_dict(retail_store_last_operation_names_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


