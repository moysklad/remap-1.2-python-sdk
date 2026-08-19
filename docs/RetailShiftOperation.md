# RetailShiftOperation

Элемент массива `operations` розничной смены. Допустимые `meta.type`: retaildemand, retailsalesreturn, retaildrawercashin, retaildrawercashout, prepayment, prepaymentreturn. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift_operation import RetailShiftOperation

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShiftOperation from a JSON string
retail_shift_operation_instance = RetailShiftOperation.from_json(json)
# print the JSON string representation of the object
print(RetailShiftOperation.to_json())

# convert the object into a dict
retail_shift_operation_dict = retail_shift_operation_instance.to_dict()
# create an instance of RetailShiftOperation from a dict
retail_shift_operation_from_dict = RetailShiftOperation.from_dict(retail_shift_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


