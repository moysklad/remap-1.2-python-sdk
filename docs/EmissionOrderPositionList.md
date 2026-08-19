# EmissionOrderPositionList

Список позиций Заказа кодов маркировки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[EmissionOrderPosition]**](EmissionOrderPosition.md) | Массив позиций Заказа кодов маркировки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.emission_order_position_list import EmissionOrderPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionOrderPositionList from a JSON string
emission_order_position_list_instance = EmissionOrderPositionList.from_json(json)
# print the JSON string representation of the object
print(EmissionOrderPositionList.to_json())

# convert the object into a dict
emission_order_position_list_dict = emission_order_position_list_instance.to_dict()
# create an instance of EmissionOrderPositionList from a dict
emission_order_position_list_from_dict = EmissionOrderPositionList.from_dict(emission_order_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


