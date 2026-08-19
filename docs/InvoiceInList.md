# InvoiceInList

Список Счетов поставщикам

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[InvoiceIn]**](InvoiceIn.md) | Массив Счетов поставщикам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.invoice_in_list import InvoiceInList

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceInList from a JSON string
invoice_in_list_instance = InvoiceInList.from_json(json)
# print the JSON string representation of the object
print(InvoiceInList.to_json())

# convert the object into a dict
invoice_in_list_dict = invoice_in_list_instance.to_dict()
# create an instance of InvoiceInList from a dict
invoice_in_list_from_dict = InvoiceInList.from_dict(invoice_in_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


