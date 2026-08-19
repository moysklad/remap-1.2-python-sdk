# PurchaseOrderRate

Валюта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | [**Currency**](Currency.md) |  | [optional] 
**value** | **float** | Курс валюты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_order_rate import PurchaseOrderRate

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderRate from a JSON string
purchase_order_rate_instance = PurchaseOrderRate.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderRate.to_json())

# convert the object into a dict
purchase_order_rate_dict = purchase_order_rate_instance.to_dict()
# create an instance of PurchaseOrderRate from a dict
purchase_order_rate_from_dict = PurchaseOrderRate.from_dict(purchase_order_rate_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


