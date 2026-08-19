# RetailStoreStateFiscalMemory

Статус фискальной памяти

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | [**RetailStoreStateFiscalMemoryError**](RetailStoreStateFiscalMemoryError.md) |  | [optional] 
**not_send_doc_count** | **int** | Количество неотправленных документов | [optional] 
**not_send_first_doc_moment** | **str** | Момент первого неотправленного документа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_state_fiscal_memory import RetailStoreStateFiscalMemory

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreStateFiscalMemory from a JSON string
retail_store_state_fiscal_memory_instance = RetailStoreStateFiscalMemory.from_json(json)
# print the JSON string representation of the object
print(RetailStoreStateFiscalMemory.to_json())

# convert the object into a dict
retail_store_state_fiscal_memory_dict = retail_store_state_fiscal_memory_instance.to_dict()
# create an instance of RetailStoreStateFiscalMemory from a dict
retail_store_state_fiscal_memory_from_dict = RetailStoreStateFiscalMemory.from_dict(retail_store_state_fiscal_memory_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


