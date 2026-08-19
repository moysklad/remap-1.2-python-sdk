# PurchaseOrderList

Список Заказов поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[PurchaseOrder]**](PurchaseOrder.md) | Массив Заказов поставщику | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_order_list import PurchaseOrderList

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderList from a JSON string
purchase_order_list_instance = PurchaseOrderList.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderList.to_json())

# convert the object into a dict
purchase_order_list_dict = purchase_order_list_instance.to_dict()
# create an instance of PurchaseOrderList from a dict
purchase_order_list_from_dict = PurchaseOrderList.from_dict(purchase_order_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


