# PurchaseOrderPositionList

Список позиций Заказа поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[PurchaseOrderPosition]**](PurchaseOrderPosition.md) | Массив позиций Заказа поставщику | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_order_position_list import PurchaseOrderPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseOrderPositionList from a JSON string
purchase_order_position_list_instance = PurchaseOrderPositionList.from_json(json)
# print the JSON string representation of the object
print(PurchaseOrderPositionList.to_json())

# convert the object into a dict
purchase_order_position_list_dict = purchase_order_position_list_instance.to_dict()
# create an instance of PurchaseOrderPositionList from a dict
purchase_order_position_list_from_dict = PurchaseOrderPositionList.from_dict(purchase_order_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


