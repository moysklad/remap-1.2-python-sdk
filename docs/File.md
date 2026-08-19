# File

Файл

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**title** | **str** | Название файла | [optional] 
**filename** | **str** | Имя файла | [optional] 
**content** | **str** | Файл, закодированный в Base64 | [optional] 
**size** | **int** | Размер файла в байтах | [optional] [readonly] 
**created** | **str** | Время создания объекта | [optional] [readonly] 
**created_by** | [**Employee**](Employee.md) |  | [optional] 
**tiny** | [**Meta**](Meta.md) |  | [optional] 
**miniature** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.file import File

# TODO update the JSON string below
json = "{}"
# create an instance of File from a JSON string
file_instance = File.from_json(json)
# print the JSON string representation of the object
print(File.to_json())

# convert the object into a dict
file_dict = file_instance.to_dict()
# create an instance of File from a dict
file_from_dict = File.from_dict(file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


