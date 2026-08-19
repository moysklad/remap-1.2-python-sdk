# PrepaymentReturnList

Список Возвратов предоплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[PrepaymentReturn]**](PrepaymentReturn.md) | Массив Возвратов предоплаты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.prepayment_return_list import PrepaymentReturnList

# TODO update the JSON string below
json = "{}"
# create an instance of PrepaymentReturnList from a JSON string
prepayment_return_list_instance = PrepaymentReturnList.from_json(json)
# print the JSON string representation of the object
print(PrepaymentReturnList.to_json())

# convert the object into a dict
prepayment_return_list_dict = prepayment_return_list_instance.to_dict()
# create an instance of PrepaymentReturnList from a dict
prepayment_return_list_from_dict = PrepaymentReturnList.from_dict(prepayment_return_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


