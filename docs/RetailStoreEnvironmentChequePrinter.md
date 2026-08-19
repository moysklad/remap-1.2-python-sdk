# RetailStoreEnvironmentChequePrinter

Информация о чековом принтере

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**driver** | [**RetailStoreEnvironmentChequePrinterDriver**](RetailStoreEnvironmentChequePrinterDriver.md) |  | [optional] 
**firmware_version** | **str** | Версия прошивки | [optional] 
**fiscal_data_version** | **str** | Версия фискальных данных | [optional] 
**fiscal_memory** | [**RetailStoreEnvironmentChequePrinterFiscalMemory**](RetailStoreEnvironmentChequePrinterFiscalMemory.md) |  | [optional] 
**name** | **str** | Наименование чекового принтера | [optional] 
**serial** | **str** | Серийный номер чекового принтера | [optional] 
**vendor** | **str** | Производитель чекового принтера | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_store_environment_cheque_printer import RetailStoreEnvironmentChequePrinter

# TODO update the JSON string below
json = "{}"
# create an instance of RetailStoreEnvironmentChequePrinter from a JSON string
retail_store_environment_cheque_printer_instance = RetailStoreEnvironmentChequePrinter.from_json(json)
# print the JSON string representation of the object
print(RetailStoreEnvironmentChequePrinter.to_json())

# convert the object into a dict
retail_store_environment_cheque_printer_dict = retail_store_environment_cheque_printer_instance.to_dict()
# create an instance of RetailStoreEnvironmentChequePrinter from a dict
retail_store_environment_cheque_printer_from_dict = RetailStoreEnvironmentChequePrinter.from_dict(retail_store_environment_cheque_printer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


