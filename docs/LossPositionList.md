# LossPositionList

Список позиций Списания

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[LossPosition]**](LossPosition.md) | Массив позиций Списания | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.loss_position_list import LossPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of LossPositionList from a JSON string
loss_position_list_instance = LossPositionList.from_json(json)
# print the JSON string representation of the object
print(LossPositionList.to_json())

# convert the object into a dict
loss_position_list_dict = loss_position_list_instance.to_dict()
# create an instance of LossPositionList from a dict
loss_position_list_from_dict = LossPositionList.from_dict(loss_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


