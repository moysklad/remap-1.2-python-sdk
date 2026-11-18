# PurchaseReturnPayment

Элемент массива `payments` возврата поставщику. Допустимые `meta.type`: paymentin, cashin. Поле `linkedSum` сохраняется у элемента связи. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_return_payment import PurchaseReturnPayment

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseReturnPayment from a JSON string
purchase_return_payment_instance = PurchaseReturnPayment.from_json(json)
# print the JSON string representation of the object
print(PurchaseReturnPayment.to_json())

# convert the object into a dict
purchase_return_payment_dict = purchase_return_payment_instance.to_dict()
# create an instance of PurchaseReturnPayment from a dict
purchase_return_payment_from_dict = PurchaseReturnPayment.from_dict(purchase_return_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


