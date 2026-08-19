# DeleteInvoiceOutBatch200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**info** | **str** | Информационное сообщение об удалении сущности | [optional] 
**errors** | [**List[ErrorErrorsInner]**](ErrorErrorsInner.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.delete_invoice_out_batch200_response_inner import DeleteInvoiceOutBatch200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteInvoiceOutBatch200ResponseInner from a JSON string
delete_invoice_out_batch200_response_inner_instance = DeleteInvoiceOutBatch200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(DeleteInvoiceOutBatch200ResponseInner.to_json())

# convert the object into a dict
delete_invoice_out_batch200_response_inner_dict = delete_invoice_out_batch200_response_inner_instance.to_dict()
# create an instance of DeleteInvoiceOutBatch200ResponseInner from a dict
delete_invoice_out_batch200_response_inner_from_dict = DeleteInvoiceOutBatch200ResponseInner.from_dict(delete_invoice_out_batch200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


