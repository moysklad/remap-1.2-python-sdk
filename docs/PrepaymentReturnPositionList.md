# PrepaymentReturnPositionList

Список позиций Возврата предоплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[PrepaymentReturnPosition]**](PrepaymentReturnPosition.md) | Массив позиций Возврата предоплаты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.prepayment_return_position_list import PrepaymentReturnPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of PrepaymentReturnPositionList from a JSON string
prepayment_return_position_list_instance = PrepaymentReturnPositionList.from_json(json)
# print the JSON string representation of the object
print(PrepaymentReturnPositionList.to_json())

# convert the object into a dict
prepayment_return_position_list_dict = prepayment_return_position_list_instance.to_dict()
# create an instance of PrepaymentReturnPositionList from a dict
prepayment_return_position_list_from_dict = PrepaymentReturnPositionList.from_dict(prepayment_return_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


