# InvoiceOutList

Список Счетов покупателям

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[InvoiceOut]**](InvoiceOut.md) | Массив Счетов покупателям | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.invoice_out_list import InvoiceOutList

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceOutList from a JSON string
invoice_out_list_instance = InvoiceOutList.from_json(json)
# print the JSON string representation of the object
print(InvoiceOutList.to_json())

# convert the object into a dict
invoice_out_list_dict = invoice_out_list_instance.to_dict()
# create an instance of InvoiceOutList from a dict
invoice_out_list_from_dict = InvoiceOutList.from_dict(invoice_out_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


