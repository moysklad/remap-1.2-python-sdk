# PurchaseOrderPayment

Элемент массива `payments` документа purchaseOrder. Ссылка или раскрытый платеж; `linkedSum` может отсутствовать. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**linked_sum** | **float** | Сумма, оплаченная по данному документу; может отсутствовать у ссылки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_order_payment import PurchaseOrderPayment

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderPayment from a JSON string
purchase_order_payment_instance = PurchaseOrderPayment.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderPayment.to_json())

# convert the object into a dict
purchase_order_payment_dict = purchase_order_payment_instance.to_dict()
# create an instance of PurchaseOrderPayment from a dict
purchase_order_payment_from_dict = PurchaseOrderPayment.from_dict(purchase_order_payment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


