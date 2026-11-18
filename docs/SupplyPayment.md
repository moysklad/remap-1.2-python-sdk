# SupplyPayment

Платеж, связанный с приемкой: исходящий платеж или расходный ордер. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.supply_payment import SupplyPayment

# TODO update the JSON string below
json = "{}"
# create an instance of SupplyPayment from a JSON string
supply_payment_instance = SupplyPayment.from_json(json)
# print the JSON string representation of the object
print(SupplyPayment.to_json())

# convert the object into a dict
supply_payment_dict = supply_payment_instance.to_dict()
# create an instance of SupplyPayment from a dict
supply_payment_from_dict = SupplyPayment.from_dict(supply_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


