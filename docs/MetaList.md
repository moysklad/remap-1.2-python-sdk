# MetaList

Метаданные списка

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** | Ссылка на объект | 
**type** | **str** | Тип объекта | 
**media_type** | **str** | Тип данных | 
**size** | **int** | Размер выданного списка | [optional] 
**limit** | **int** | Максимальное количество элементов в выданном списке | [optional] 
**offset** | **int** | Отступ в выданном списке | [optional] 
**next_href** | **str** | Ссылка на следующую страницу | [optional] 
**previous_href** | **str** | Ссылка на предыдущую страницу | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.meta_list import MetaList

# TODO update the JSON string below
json = "{}"
# create an instance of MetaList from a JSON string
meta_list_instance = MetaList.from_json(json)
# print the JSON string representation of the object
print(MetaList.to_json())

# convert the object into a dict
meta_list_dict = meta_list_instance.to_dict()
# create an instance of MetaList from a dict
meta_list_from_dict = MetaList.from_dict(meta_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


