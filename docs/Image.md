# Image

Изображение

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**title** | **str** | Название изображения | [optional] 
**filename** | **str** | Имя файла | [optional] 
**content** | **str** | Изображение, закодированное в Base64 | [optional] 
**size** | **int** | Размер файла в байтах | [optional] [readonly] 
**updated** | **str** | Время последнего изменения | [optional] [readonly] 
**tiny** | [**Meta**](Meta.md) |  | [optional] 
**miniature** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.image import Image

# TODO update the JSON string below
json = "{}"
# create an instance of Image from a JSON string
image_instance = Image.from_json(json)
# print the JSON string representation of the object
print(Image.to_json())

# convert the object into a dict
image_dict = image_instance.to_dict()
# create an instance of Image from a dict
image_from_dict = Image.from_dict(image_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


