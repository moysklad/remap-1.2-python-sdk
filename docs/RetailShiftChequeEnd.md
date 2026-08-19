# RetailShiftChequeEnd

Информация о закрытии смены ККТ

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cheques_total** | **int** | Количество чеков за смену | [optional] 
**fiscal_doc_number** | **str** | Номер фискального документа | [optional] 
**fiscal_doc_sign** | **str** | Фискальный признак документа | [optional] 
**fiscal_docs_total** | **int** | Количество фискальных документов за смену | [optional] 
**fn_number** | **str** | Номер фискального накопителя | [optional] 
**kkt_reg_number** | **str** | Регистрационный номер ККТ | [optional] 
**shift_number** | **str** | Номер смены ККТ | [optional] 
**time** | **str** | Дата и время закрытия смены | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift_cheque_end import RetailShiftChequeEnd

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShiftChequeEnd from a JSON string
retail_shift_cheque_end_instance = RetailShiftChequeEnd.from_json(json)
# print the JSON string representation of the object
print(RetailShiftChequeEnd.to_json())

# convert the object into a dict
retail_shift_cheque_end_dict = retail_shift_cheque_end_instance.to_dict()
# create an instance of RetailShiftChequeEnd from a dict
retail_shift_cheque_end_from_dict = RetailShiftChequeEnd.from_dict(retail_shift_cheque_end_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


