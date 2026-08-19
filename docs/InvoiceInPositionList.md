# InvoiceInPositionList

Список позиций Счета поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[InvoiceInPosition]**](InvoiceInPosition.md) | Массив позиций Счета поставщику | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.invoice_in_position_list import InvoiceInPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceInPositionList from a JSON string
invoice_in_position_list_instance = InvoiceInPositionList.from_json(json)
# print the JSON string representation of the object
print(InvoiceInPositionList.to_json())

# convert the object into a dict
invoice_in_position_list_dict = invoice_in_position_list_instance.to_dict()
# create an instance of InvoiceInPositionList from a dict
invoice_in_position_list_from_dict = InvoiceInPositionList.from_dict(invoice_in_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


