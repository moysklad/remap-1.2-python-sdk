# CustomEntityElementList

Список элементов пользовательского справочника

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CustomEntityElement]**](CustomEntityElement.md) | Массив элементов пользовательского справочника | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.custom_entity_element_list import CustomEntityElementList

# TODO update the JSON string below
json = "{}"
# create an instance of CustomEntityElementList from a JSON string
custom_entity_element_list_instance = CustomEntityElementList.from_json(json)
# print the JSON string representation of the object
print(CustomEntityElementList.to_json())

# convert the object into a dict
custom_entity_element_list_dict = custom_entity_element_list_instance.to_dict()
# create an instance of CustomEntityElementList from a dict
custom_entity_element_list_from_dict = CustomEntityElementList.from_dict(custom_entity_element_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


