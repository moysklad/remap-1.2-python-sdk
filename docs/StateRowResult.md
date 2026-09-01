# StateRowResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID статуса | [optional] [readonly] 
**name** | **str** | Наименование статуса | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**color** | **int** | Цвет Статуса | [optional] 
**entity_type** | **str** | Тип сущности, к которой относится Статус (ключевое слово в рамках JSON API) | [optional] [readonly] 
**state_type** | **str** | Тип Статуса. Известные значения описаны в StateType | [optional] 
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.state_row_result import StateRowResult

# TODO update the JSON string below
json = "{}"
# create an instance of StateRowResult from a JSON string
state_row_result_instance = StateRowResult.from_json(json)
# print the JSON string representation of the object
print(StateRowResult.to_json())

# convert the object into a dict
state_row_result_dict = state_row_result_instance.to_dict()
# create an instance of StateRowResult from a dict
state_row_result_from_dict = StateRowResult.from_dict(state_row_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


