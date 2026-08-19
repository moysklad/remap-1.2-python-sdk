# RetailStoreEnvironmentChequePrinterFiscalMemory

Фискальная память

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fiscal_data_version** | **str** | Версия фискальных данных | [optional] 
**fiscal_validity_date** | **str** | Дата окончания действия фискальной памяти | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_environment_cheque_printer_fiscal_memory import RetailStoreEnvironmentChequePrinterFiscalMemory

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreEnvironmentChequePrinterFiscalMemory from a JSON string
retail_store_environment_cheque_printer_fiscal_memory_instance = RetailStoreEnvironmentChequePrinterFiscalMemory.from_json(json)
# print the JSON string representation of the object
print(RetailStoreEnvironmentChequePrinterFiscalMemory.to_json())

# convert the object into a dict
retail_store_environment_cheque_printer_fiscal_memory_dict = retail_store_environment_cheque_printer_fiscal_memory_instance.to_dict()
# create an instance of RetailStoreEnvironmentChequePrinterFiscalMemory from a dict
retail_store_environment_cheque_printer_fiscal_memory_from_dict = RetailStoreEnvironmentChequePrinterFiscalMemory.from_dict(retail_store_environment_cheque_printer_fiscal_memory_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


