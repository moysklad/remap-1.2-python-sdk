# FactureOutPayment

Платеж, связанный со счетом-фактурой выданным: входящий платеж или приходный ордер. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.facture_out_payment import FactureOutPayment

# TODO update the JSON string below
json = "{}"
# create an instance of FactureOutPayment from a JSON string
facture_out_payment_instance = FactureOutPayment.from_json(json)
# print the JSON string representation of the object
print(FactureOutPayment.to_json())

# convert the object into a dict
facture_out_payment_dict = facture_out_payment_instance.to_dict()
# create an instance of FactureOutPayment from a dict
facture_out_payment_from_dict = FactureOutPayment.from_dict(facture_out_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


