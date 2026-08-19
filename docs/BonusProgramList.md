# BonusProgramList

Список бонусных программ

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[BonusProgram]**](BonusProgram.md) | Массив бонусных программ | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bonus_program_list import BonusProgramList

# TODO update the JSON string below
json = "{}"
# create an instance of BonusProgramList from a JSON string
bonus_program_list_instance = BonusProgramList.from_json(json)
# print the JSON string representation of the object
print(BonusProgramList.to_json())

# convert the object into a dict
bonus_program_list_dict = bonus_program_list_instance.to_dict()
# create an instance of BonusProgramList from a dict
bonus_program_list_from_dict = BonusProgramList.from_dict(bonus_program_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


