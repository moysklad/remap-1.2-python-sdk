# RetailStoreStatePaymentTerminal

Информация о платежном терминале

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acquiring_type** | **str** | Тип эквайринга | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_state_payment_terminal import RetailStoreStatePaymentTerminal

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreStatePaymentTerminal from a JSON string
retail_store_state_payment_terminal_instance = RetailStoreStatePaymentTerminal.from_json(json)
# print the JSON string representation of the object
print(RetailStoreStatePaymentTerminal.to_json())

# convert the object into a dict
retail_store_state_payment_terminal_dict = retail_store_state_payment_terminal_instance.to_dict()
# create an instance of RetailStoreStatePaymentTerminal from a dict
retail_store_state_payment_terminal_from_dict = RetailStoreStatePaymentTerminal.from_dict(retail_store_state_payment_terminal_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


