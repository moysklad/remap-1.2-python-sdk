# RetailShiftCheque

Информация о смене ККТ

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start** | [**RetailShiftChequeStart**](RetailShiftChequeStart.md) |  | [optional] 
**end** | [**RetailShiftChequeEnd**](RetailShiftChequeEnd.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift_cheque import RetailShiftCheque

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShiftCheque from a JSON string
retail_shift_cheque_instance = RetailShiftCheque.from_json(json)
# print the JSON string representation of the object
print(RetailShiftCheque.to_json())

# convert the object into a dict
retail_shift_cheque_dict = retail_shift_cheque_instance.to_dict()
# create an instance of RetailShiftCheque from a dict
retail_shift_cheque_from_dict = RetailShiftCheque.from_dict(retail_shift_cheque_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


