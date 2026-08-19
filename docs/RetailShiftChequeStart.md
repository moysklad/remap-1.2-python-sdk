# RetailShiftChequeStart

Информация об открытии смены ККТ

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fn_number** | **str** | Номер фискального накопителя | [optional] 
**kkt_reg_number** | **str** | Регистрационный номер ККТ | [optional] 
**fiscal_doc_sign** | **str** | Фискальный признак документа | [optional] 
**shift_number** | **str** | Номер смены ККТ | [optional] 
**fiscal_doc_number** | **str** | Номер фискального документа | [optional] 
**time** | **str** | Дата и время открытия смены | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift_cheque_start import RetailShiftChequeStart

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShiftChequeStart from a JSON string
retail_shift_cheque_start_instance = RetailShiftChequeStart.from_json(json)
# print the JSON string representation of the object
print(RetailShiftChequeStart.to_json())

# convert the object into a dict
retail_shift_cheque_start_dict = retail_shift_cheque_start_instance.to_dict()
# create an instance of RetailShiftChequeStart from a dict
retail_shift_cheque_start_from_dict = RetailShiftChequeStart.from_dict(retail_shift_cheque_start_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


