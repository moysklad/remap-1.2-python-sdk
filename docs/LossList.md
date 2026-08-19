# LossList

Список Списаний

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Loss]**](Loss.md) | Массив Списаний | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.loss_list import LossList

# TODO update the JSON string below
json = "{}"
# create an instance of LossList from a JSON string
loss_list_instance = LossList.from_json(json)
# print the JSON string representation of the object
print(LossList.to_json())

# convert the object into a dict
loss_list_dict = loss_list_instance.to_dict()
# create an instance of LossList from a dict
loss_list_from_dict = LossList.from_dict(loss_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


