# PurchaseReturnPositionList

Список позиций Возврата поставщику

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[PurchaseReturnPosition]**](PurchaseReturnPosition.md) | Массив позиций Возврата поставщику | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_return_position_list import PurchaseReturnPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseReturnPositionList from a JSON string
purchase_return_position_list_instance = PurchaseReturnPositionList.from_json(json)
# print the JSON string representation of the object
print(PurchaseReturnPositionList.to_json())

# convert the object into a dict
purchase_return_position_list_dict = purchase_return_position_list_instance.to_dict()
# create an instance of PurchaseReturnPositionList from a dict
purchase_return_position_list_from_dict = PurchaseReturnPositionList.from_dict(purchase_return_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


