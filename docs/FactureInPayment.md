# FactureInPayment

Платеж, связанный со счетом-фактурой полученным: исходящий платеж или расходный ордер. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.facture_in_payment import FactureInPayment

# TODO update the JSON string below
json = "{}"
# create an instance of FactureInPayment from a JSON string
facture_in_payment_instance = FactureInPayment.from_json(json)
# print the JSON string representation of the object
print(FactureInPayment.to_json())

# convert the object into a dict
facture_in_payment_dict = facture_in_payment_instance.to_dict()
# create an instance of FactureInPayment from a dict
facture_in_payment_from_dict = FactureInPayment.from_dict(facture_in_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


