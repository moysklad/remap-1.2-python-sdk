# RetailShiftPayment

Элемент массива `payments` документа retailShift. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift_payment import RetailShiftPayment

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShiftPayment from a JSON string
retail_shift_payment_instance = RetailShiftPayment.from_json(json)
# print the JSON string representation of the object
print(RetailShiftPayment.to_json())

# convert the object into a dict
retail_shift_payment_dict = retail_shift_payment_instance.to_dict()
# create an instance of RetailShiftPayment from a dict
retail_shift_payment_from_dict = RetailShiftPayment.from_dict(retail_shift_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


