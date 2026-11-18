# DemandPayment

Элемент массива `payments` документа demand. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.demand_payment import DemandPayment

# TODO update the JSON string below
json = "{}"
# create an instance of DemandPayment from a JSON string
demand_payment_instance = DemandPayment.from_json(json)
# print the JSON string representation of the object
print(DemandPayment.to_json())

# convert the object into a dict
demand_payment_dict = demand_payment_instance.to_dict()
# create an instance of DemandPayment from a dict
demand_payment_from_dict = DemandPayment.from_dict(demand_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


