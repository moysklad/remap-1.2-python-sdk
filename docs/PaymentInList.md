# PaymentInList

Список Входящих платежей

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[PaymentIn]**](PaymentIn.md) | Массив Входящих платежей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.payment_in_list import PaymentInList

# TODO update the JSON string below
json = "{}"
# create an instance of PaymentInList from a JSON string
payment_in_list_instance = PaymentInList.from_json(json)
# print the JSON string representation of the object
print(PaymentInList.to_json())

# convert the object into a dict
payment_in_list_dict = payment_in_list_instance.to_dict()
# create an instance of PaymentInList from a dict
payment_in_list_from_dict = PaymentInList.from_dict(payment_in_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


