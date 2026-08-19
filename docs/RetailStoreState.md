# RetailStoreState

Статус точки продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sync** | [**RetailStoreStateSync**](RetailStoreStateSync.md) |  | [optional] 
**last_check_moment** | **str** | Момент последней проверки | [optional] 
**fiscal_memory** | [**RetailStoreStateFiscalMemory**](RetailStoreStateFiscalMemory.md) |  | [optional] 
**payment_terminal** | [**RetailStoreStatePaymentTerminal**](RetailStoreStatePaymentTerminal.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_state import RetailStoreState

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreState from a JSON string
retail_store_state_instance = RetailStoreState.from_json(json)
# print the JSON string representation of the object
print(RetailStoreState.to_json())

# convert the object into a dict
retail_store_state_dict = retail_store_state_instance.to_dict()
# create an instance of RetailStoreState from a dict
retail_store_state_from_dict = RetailStoreState.from_dict(retail_store_state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


