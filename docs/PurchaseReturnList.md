# PurchaseReturnList

Список Возвратов поставщикам

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[PurchaseReturn]**](PurchaseReturn.md) | Массив Возвратов поставщикам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.purchase_return_list import PurchaseReturnList

# TODO update the JSON string below
json = "{}"
# create an instance of PurchaseReturnList from a JSON string
purchase_return_list_instance = PurchaseReturnList.from_json(json)
# print the JSON string representation of the object
print(PurchaseReturnList.to_json())

# convert the object into a dict
purchase_return_list_dict = purchase_return_list_instance.to_dict()
# create an instance of PurchaseReturnList from a dict
purchase_return_list_from_dict = PurchaseReturnList.from_dict(purchase_return_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


