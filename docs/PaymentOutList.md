# PaymentOutList

Список Исходящих платежей

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[PaymentOut]**](PaymentOut.md) | Массив Исходящих платежей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.payment_out_list import PaymentOutList

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentOutList from a JSON string
payment_out_list_instance = PaymentOutList.from_json(json)
# print the JSON string representation of the object
print(PaymentOutList.to_json())

# convert the object into a dict
payment_out_list_dict = payment_out_list_instance.to_dict()
# create an instance of PaymentOutList from a dict
payment_out_list_from_dict = PaymentOutList.from_dict(payment_out_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


