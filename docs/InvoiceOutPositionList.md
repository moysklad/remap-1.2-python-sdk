# InvoiceOutPositionList

Список позиций Счета покупателю

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[InvoiceOutPosition]**](InvoiceOutPosition.md) | Массив позиций Счета покупателю | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.invoice_out_position_list import InvoiceOutPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceOutPositionList from a JSON string
invoice_out_position_list_instance = InvoiceOutPositionList.from_json(json)
# print the JSON string representation of the object
print(InvoiceOutPositionList.to_json())

# convert the object into a dict
invoice_out_position_list_dict = invoice_out_position_list_instance.to_dict()
# create an instance of InvoiceOutPositionList from a dict
invoice_out_position_list_from_dict = InvoiceOutPositionList.from_dict(invoice_out_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


